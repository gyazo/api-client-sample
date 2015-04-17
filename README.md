# Gyazo API Client

This app is an example of GyazoAPI client using [doorkeeper-sinatra-client](https://github.com/applicake/doorkeeper-sinatra-client)
[demo](https://api-client-sample.herokuapp.com/). 

## About Gyazo API

[resister & docs](https://gyazo.com/api), 

## Installation

First clone the [repository from GitHub](https://github.com/gyazo/api-client-sample):

    git clone git://github.com/gyazo/api-client-sample.git

Install all dependencies with:

    bundle install

### Environment variables

You need to setup few environment variables in order to make the client work. You can either set the variables in you environment:

    export OAUTH2_CLIENT_ID           = "129477f..."
    export OAUTH2_CLIENT_SECRET       = "c1eec90..."
    export OAUTH2_CLIENT_REDIRECT_URI = "http://localhost:9393/callback"


or set them in a file named `env.rb` in the app's root. This file is loaded automatically by the app.

    # env.rb
    ENV['OAUTH2_CLIENT_ID']           = "129477f..."
    ENV['OAUTH2_CLIENT_SECRET']       = "c1eec90..."
    ENV['OAUTH2_CLIENT_REDIRECT_URI'] = "http://localhost:9393/callback"

## Start the server

Fire up the server with:

    rackup config.ru
