# Synthetix Sandbox

This repository serves as a starting point for developing front-ends and smart contract integrations for [Synthetix V3](https://github.com/Synthetixio/synthetix-v3).

Install [Cannon](https://usecannon.com) with `npm i -g @usecannon/cli` an review the [Get Started guide](https://usecannon.com/get-started).

**Remember to always interact with the proxy contracts instead of the router or modules directly.**

## Developing Front-ends

* Run `cannon synthetix-sandbox` to start a local node as defined in the [Cannonfile](/cannonfile.toml) for front-end development
* Run `cannon inspect synthetix-sandbox --write-deployments ./deployments` to export the smart contract ABIs and addresses

## Developing Smart Contract Integrations

* Fork this repository
* Modify the [Sample Integration contract](/src/SampleIntegration.sol)
* Customize the name at the top of `cannonfile.toml` and make any other modifications
* Run `cannon build` 
* Run `cannon <replace-with-new-cannonfile-name>`

See the [Production Cannonfile](/cannonfile.prod.toml) for an example Cannonfile that deploys the Sample Integration contract integrated with the official [Synthetix V3 Deployments](https://github.com/Synthetixio/synthetix-deployments).
