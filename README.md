# Starter for deploying [fast.ai](https://www.fast.ai) models on Heroku

~~~~
docker image build -t <app-name> .
docker run --rm -it -p 80:8008 <app-name>
heroku container:push web -a <app-name>
heroku container:release web -a <app-name>
heroku open -a <app-name>
~~~~
