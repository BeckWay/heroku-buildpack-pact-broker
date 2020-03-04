Heroku buildpack: Pact Broker CLI
=========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that
allows one to run the [Pact Broker CLI](https://github.com/pact-foundation/pact_broker-client) in a dyno alongside application code.

Usage
-----

Add to any Heroku app:

    $ heroku buildpacks:add https://github.com/BeckWay/heroku-buildpack-pact-broker --app <MY_HEROKU_APP_NAME>

And deploy the app again to use the buildpack.

Then from your `Procfile` or elsewhere:

```
release: pact-broker can-i-deploy <options>
```
