# TypeScript Experiments

* Inspired by this tweet: https://twitter.com/_jayphelps/status/1067221396374384640

```ts
const testFunction = (a: number, b: number) => {
  if (a > b) {
    return;
  } else if (a < b) {
    return;
  } else if (a === b) {
    return;
  } else {
    throw new Error("Unreachable code");
  }
}
```

Is it possible for this code to throw an error when compiled with TypeScript?


# Run

```
cd /tmp
git clone https://github.com/ndbroadbent/typescript-experiments.git
cd typescript-experiments
yarn install
yarn run check
yarn start
```


## References

* [The Curious Case of JavaScript NaN](https://ariya.io/2014/05/the-curious-case-of-javascript-nan)
* [StackOverflow: Is it possible to make TypeScript crash on 0 / 0 and Math.log(-1) instead of returning NaN?](https://stackoverflow.com/questions/20534887/break-on-nan-in-javascript)
* [StackOverflow: Break on NaN in JavaScript](https://stackoverflow.com/questions/20534887/break-on-nan-in-javascript)
* [TypeScript Issue about adding a NaN type](https://github.com/Microsoft/TypeScript/issues/21279)
