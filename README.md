this is the TDS project 1 


use the following commands

echo $AIPROXY_TOKEN

export AIPROXY_TOKEN="eyJhbGciOiJIUzI1NiJ9.eyJlbWFpbCI6IjIyZjMwMDE1NTFAZHMuc3R1ZHkuaWl0bS5hYy5pbiJ9.BkF49EwczoSdCZlFVYsjSxDEoqI3An374-K86-0p-Mw"

docker build -t mj665/tdsp1 .


echo $AIPROXY_TOKEN


docker run --rm -e AIPROXY_TOKEN=$AIPROXY_TOKEN -p 8000:8000 mj665/tdsp1


uv run evaluate.py 


docker push mj665/tdsp1