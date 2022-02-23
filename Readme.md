
docker run -v $(pwd):/app rasa/rasa:latest init --no-prompt

docker run -it -v $(pwd):/app rasa/rasa:latest shell

docker run -v $(pwd):/app rasa/rasa:latest train --domain domain.yml --data data --out models
