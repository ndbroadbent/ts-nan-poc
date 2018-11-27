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
