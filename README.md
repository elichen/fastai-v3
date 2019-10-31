# Starter for deploying [fast.ai](https://www.fast.ai) models on Heroku

~~~~
export APPNAME="street-signs"
docker image build -t $APPNAME:latest .
docker run --rm -it -p 80:8008 $APPNAME:latest
heroku container:push web -a $APPNAME
heroku container:release web -a $APPNAME
heroku open -a $APPNAME
~~~~
