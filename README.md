

## Description

See the lab [race-condition](https://ull-mii-sytws.github.io/practicas/race-condition.html)

## The Experiment

Install  [http-server](https://www.npmjs.com/package/http-server).

Then  serve this `index.html` file with:

```
http-server -p 9000 -o
```

with this line uncommented 

```js
let waitFor = 2000;
```

Can you see the infinite loop image?

Now  comment the line where `waitFor` is initialized and uncomment the other:

```js
let waitFor = 0;
```

and run:

```
http-server -p 8000 -o
```

(Change the port to avoid cache problems)

What do you think it will happen? Can you explain it?
