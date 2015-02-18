# Unicorn + nginx on Heroku

A minimal example, based on [ryandotsmith/nginx-buildpack](https://github.com/ryandotsmith/nginx-buildpack)

Deploy it and see how keep-alive works with Unicorn on Heroku:

```
$ curl -kso /dev/null -w "tcp:%{time_connect}, ssldone:%{time_appconnect}\n" -o /dev/null https://desolate-sierra-3796.herokuapp.com/ https://desolate-sierra-3796.herokuapp.com/
tcp:0.311, ssldone:0.823
tcp:0.000, ssldone:0.000
```
