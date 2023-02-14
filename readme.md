# Hardhat Moonbeam

Following along [with this](https://docs.moonbeam.network/builders/build/eth-api/dev-env/hardhat/)


## Notes


* Private key used is the 'Gerald' prefunded dev account
* configure the dev network
* npx hardhat run --network dev scripts/deploy.js
* npx hardhat console --network dev
* my deploy - address was 0xC2Bf5F29a4384b1aB0C063e1c666f02121B6084a
    * const box = await Box.attach('0xC2Bf5F29a4384b1aB0C063e1c666f02121B6084a');

Dev network run in the usual way, e.g.

```
docker pull purestake/moonbeam:v0.29.0

docker run --rm --name moonbeam_development -p 9944:9944 -p 9933:9933 purestake/moonbeam:v0.29.0 --dev --ws-external --rpc-external
```