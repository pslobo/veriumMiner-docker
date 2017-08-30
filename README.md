# What is veriumMiner 

[veriumMiner](https://github.com/effectsToCause/veriumMiner) is a multi-threaded CPU miner for mining [Verium](https://portal.vericoin.info) using scrypt². 


## How to use this image

If you're unfamiliar with the various options available in cpuminer, you can get help by typing:

`docker container run --rm palobo/veriumminer --help`

Start mining some Verium (in background):

`docker container run -d --name [CONTAINER_NAME] palobo/veriumminer -n 1048576 -o [URL] -u [USER] -p [PASSWORD]`

An example using [Poolium](https://www.poolium.win) mining pool (there are others available):

`docker container run -d --name miner1 palobo/veriumminer -n -o stratum+tcp://vrm.poolium.win:3332 -u Weblogin.WorkerName -p WorkerPassword`

Check the containers logs to see how things are progressing:

`docker container logs -f [CONTAINER_NAME]`

## Donations

If you'd like to thank my work in dockerizing veriumMiner, donations are accepted in a number of currencies:

- BTC: `1GKzyV59tiW6gLUd9DKTcGqE15g9UUr2EL`
- ETH: `0x1F72BFc6fCDF120706417E4610327742b7169eB6`
- LTC: `LWwu11R6SyMKDdWF8b3wNv6CMw1WHMriDP`
