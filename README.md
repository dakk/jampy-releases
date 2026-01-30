# jampy-releases

![CI Status](https://github.com/dakk/jampy-releases/actions/workflows/ci.yaml/badge.svg)
![Conformance Status](https://github.com/dakk/jampy-releases/actions/workflows/conformance.yaml/badge.svg)
![Conformance Status M1](https://github.com/dakk/jampy-releases/actions/workflows/conformance_m1.yaml/badge.svg)
![JTV Status](https://github.com/dakk/jampy-releases/actions/workflows/jtv.yaml/badge.svg)
![MiniFuzz Status](https://github.com/dakk/jampy-releases/actions/workflows/minifuzz.yaml/badge.svg)

This repository contains the fuzzer-target for jampy, for different version of the gray paper.
This repository will be integrated in jampy source repository once the project will be public.


## Target

```
usage: jampy-target-0.7.2_x86-64 [-h] [--env {tiny,full}] [--socket-file SOCKET_FILE] [--version]

Jampy target

options:
  -h, --help            show this help message and exit
  --env {tiny,full}     Specify environment mode: 'tiny' or 'full' (default: 'tiny')
  --socket-file SOCKET_FILE
                        Specify the socket file (default: '/tmp/jam_target.sock')
  --version             Print the jampy and jam version and exit
```

## Fuzzer

```
usage: jampy-fuzzer-0.7.2_x86-64 [-h] [--env {tiny,full}] [--socket-file SOCKET_FILE] [--version] [--seed SEED] [--blocks BLOCKS] [--mod {fallback,safrole}]
                                 [--single-trace SINGLE_TRACE]

Jampy fuzzer

options:
  -h, --help            show this help message and exit
  --env {tiny,full}     Specify environment mode: 'tiny' or 'full' (default: 'tiny')
  --socket-file SOCKET_FILE
                        Specify the socket file (default: '/tmp/jam_target.sock')
  --version             Print the jampy and jam version and exit
  --seed SEED           Random seed (default: current timestamp)
  --blocks BLOCKS       Number of blocks (default: 10)
  --mod {fallback,safrole}
                        Fuzzer modality between 'fallback' and 'safrole' (default: fallback)
  --single-trace SINGLE_TRACE
                        Send a single trace file to the target in json or binary format (default: none)
```


## About the author

Davide Gessa (dakk(k)*)
- https://twitter.com/dagide
- https://mastodon.social/@dagide 
- https://dakk.github.io/
- https://medium.com/@dakk

View the timestamping of this repo on the [Polkadot blockchain](https://polkadot.subscan.io/account/12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV?tab=extrinsic).

Donate at: 12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV
