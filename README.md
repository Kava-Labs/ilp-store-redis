# ILP Store Redis

> ILP store for the connector, using redis as a backend

### Install

```shell
npm i @kava-labs/ilp-store-redis
```

### Usage

```js
const Store = require('@kava-labs/ilp-store-redis')
const redisStore = new Store({
  path: 'test.example', // used as prefix for keys and publish
  port: 6379 // extra arguments are passed to `ioredis` constructor
})

await redisStore.get(key)
await redisStore.put(key, value)
await redisStore.del(key)
```
