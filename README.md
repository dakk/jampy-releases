# jampy-releases

This repository contains the fuzzer-target for jampy, for different version of the gray paper.
This repository will be integrated in jampy source repository once the project will be public.

```
usage: jampy-fuzzer-target [-h] [--env {tiny,full}] [--socket-file SOCKET_FILE] [--version]

Jampy fuzzer target

options:
  -h, --help            show this help message and exit
  --env {tiny,full}     Specify environment mode: 'tiny' or 'full' (default: 'tiny')
  --socket-file SOCKET_FILE
                        Specify the socket file (default: '/tmp/jam_target.sock')
  --version             Print the jampy and jam version and exit
```

## Run on docker

```
cd docker
docker build -t jam_fuzzer .
docker run --rm -v /tmp/jam_target.sock:/tmp/jam_target.sock jam_fuzzer
```

## About the author

Davide Gessa (dakk(k)*)
- https://twitter.com/dagide
- https://mastodon.social/@dagide 
- https://dakk.github.io/
- https://medium.com/@dakk

View the timestamping of this repo on the [Polkadot blockchain](https://polkadot.subscan.io/account/12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV?tab=extrinsic).

Donate at: 12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV