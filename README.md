## Introduction
This repository contains Kyber utils smart contracts.
For more details, please visit our [developer portal](https://developer.kyber.network/)

## Package Manager
We use `yarn` as the package manager. You may use `npm` and `npx` instead, but commands in bash scripts may have to be changed accordingly.

## Setup
1. Clone this repo
2. `yarn`

## Compilation with Buidler
1. `yarn compile` to compile contracts for all solidity versions.
2. `yarn compileSol6` to compile only sol6 contracts

## Testing with Buidler
1. If contracts have not been compiled, run `yarn compile`. This step can be skipped subsequently.
2. Run full regression `yarn test`
3. Use `./test.sh -f` for running a specific test file.

### Example Commands
- `yarn test` (Runs all tests)
- `yarn buidler test --no-compile ./test/sol6/utils5.js` (Test only utils5.js for sol6)
or
- `./test.sh -f ./test/sol6/utils5.js` (Test only utils5.js for sol6)

## Coverage with `buidler-coverage`
1. Run `yarn converage`
2. Use `./coverage.sh -f` for running a specific test file.

### Example Commands
- `yarn coverage` (Runs coverage for all applicable files)
`./coverage.sh -f ./test/sol6/utils5.js` (Coverage for only utils5.js)
