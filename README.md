 # Real Time Web With Node.js
  
This is the code for the [Real Time Web with Node.js][realtime] demo app, __chattr__.

## Getting Started

To run the server you'll need [Node.js](http://nodejs.org) and [Redis](http://redis.io) installed. Then run the following commands:

1. `$ npm install`
1. `$ redis-server &`
1. `$ node app.js`

At this point you will be able to go to the address `http://localhost:8000/` in your web browser to interact with the app.

To insert messages from a command prompt

```
redis-cli

lpush messages '{"name":"terminal","data":"yo!"}'

lrange message 0 -1
```

stop redis with

```
shutdown [NOSAVE|SAVE]
```
## Inserting messages into redis using redis-cli

```
$redis-cli

LRANGE 0 -1

LPUSH messages '{"name....}"


to be continued...

