# Remittance ÐAPP 


[![Remittance YouTube Video](readme.png)](https://youtu.be/-ZW1Wp2MhnM "Remittance ÐAPP Video")

Remittance ÐAPP is an Ethereum blockchain application that allows a contributor to store funds for a beneficiary within a "lockbox".  The beneficiary may then claim the funds using valid credentials so long as they are withdrawn before the lockbox claim deadline.  Two factor authentication protects the lockbox funds, but the contributor does not submit passwords in the clear to the underlying smart contract.  The contributor may also reclaim the funds once the deadline for a lockbox has elapsed.  Administrative features such as emergency stop, deadline configuration, owner fee configuration, and emergency fund recovery; are also supported by the smart contract. 

### How tos?

##### Install dependencies

* [npm](https://www.npmjs.com/get-npm)
* [ganache-cli](https://github.com/trufflesuite/ganache-cli)

##### Running in development mode
1. Install dependencies from `package.json`
```bash
% npm install
```
2. Run `ganache-cli` (different terminal or in background)
```bash
% ganache-cli #=> will run in port 8545
OR
% ganache-cli -p <preferred port>
```
3. Truffle Compile, Migrate and Webpack mode selection
```bash
% yarn builddev
```
4. Start to serve
```
% yarn start
yarn run v1.10.1
$ http-serve /build/app
Starting up http-serve for /build/app
Available on:
  http://127.0.0.1:8080
  http://172.16.3.154:8080
  http://172.16.1.177:8080
Hit CTRL-C to stop the server
```