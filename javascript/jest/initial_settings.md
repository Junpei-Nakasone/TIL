### Install jest(for TypeScript):

Install required libraries.
```bash
npm install --save-dev jest @types/jest ts-jest
```
- jest: Testing library.
- @types/jest: Type defined file for Jest API.
- ts-jest: Tool for executing TypeScript test code without advanced compiling.

### Generate basic config file
With below command, `jest.config.js` file will be generated and it specifies that `ts-jest` is preset of jest.
```bash
npx ts-jest config:init
```
jest.config.js
```js
module.exports = {
  preset: 'ts-jest',
  testEnvironment: 'node',
};
```
