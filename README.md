# jampy-releases

![CI Status](https://github.com/dakk/jampy-releases/actions/workflows/ci.yaml/badge.svg)
![Conformance Status](https://github.com/dakk/jampy-releases/actions/workflows/conformance.yaml/badge.svg)
![Conformance Status (Docker)](https://github.com/dakk/jampy-releases/actions/workflows/conformance_docker.yaml/badge.svg)
![Conformance Status M1](https://github.com/dakk/jampy-releases/actions/workflows/conformance_m1.yaml/badge.svg)
![JTV Status](https://github.com/dakk/jampy-releases/actions/workflows/jtv.yaml/badge.svg)
![JTV Status (Docker)](https://github.com/dakk/jampy-releases/actions/workflows/jtv_docker.yaml/badge.svg)
![MiniFuzz Status](https://github.com/dakk/jampy-releases/actions/workflows/minifuzz.yaml/badge.svg)
![MiniFuzz Status (Docker)](https://github.com/dakk/jampy-releases/actions/workflows/minifuzz_docker.yaml/badge.svg)

This repository contains the fuzzer-target for jampy, for different version of the gray paper.
This repository will be integrated in jampy source repository once the project will be public.


## Target

```bash
docker pull ghcr.io/dakk/jampy-target:0.7.2
docker run ghcr.io/dakk/jampy-target:0.7.2
```

```
usage: jampy-target-0.7.2_x86-64 [-h] [--spec {tiny,full}] [--sock SOCK]
                                 [--data-dir DATA_DIR]
                                 [--log-level {error,warn,info,debug,trace}]
                                 [--version] [--trace] [--trace-pvm]
                                 [--use-recompiler]

Jampy target

options:
  -h, --help            show this help message and exit
  --spec {tiny,full}    Set chain specs: 'tiny' or 'full' (default: 'tiny' or
                        JAM_FUZZ_SPEC)
  --sock SOCK           Specify the socket file (default:
                        '/tmp/jam_target.sock' or JAM_FUZZ_SOCK_PATH)
  --data-dir DATA_DIR   Specify the data dir (default: '/tmp/jam_fuzz/' or
                        JAM_FUZZ_DATA_PATH)
  --log-level {error,warn,info,debug,trace}
                        Log verbosity: `error`, `warn`, `info`, `debug`,
                        `trace` (default: 'info' or JAM_FUZZ_LOG_LEVEL)
  --version             Print the jampy and jam version and exit
  --trace               Save a log trace on trace.txt
  --trace-pvm           Save a full pvm log trace on trace.txt
  --use-recompiler      Enable the PVM recompiler (experimental)
```

## Fuzzer

```bash
docker pull ghcr.io/dakk/jampy-fuzzer:0.7.2
docker run ghcr.io/dakk/jampy-fuzzer:0.7.2
```

```
usage: jampy-fuzzer-0.7.2_x86-64 [-h] [--spec {tiny,full}] [--sock SOCK]
                                 [--version] [--seed SEED] [--blocks BLOCKS]
                                 [--mod {fallback,safrole}]
                                 [--single-trace SINGLE_TRACE]

Jampy fuzzer

options:
  -h, --help            show this help message and exit
  --spec {tiny,full}    Set chain specs: 'tiny' or 'full' (default: 'tiny')
  --sock SOCK           Specify the socket file (default:
                        '/tmp/jam_target.sock')
  --version             Print the jampy and jam version and exit
  --seed SEED           Random seed (default: current timestamp)
  --blocks BLOCKS       Number of blocks (default: 10)
  --mod {fallback,safrole}
                        Fuzzer modality between 'fallback' and 'safrole'
                        (default: fallback)
  --single-trace SINGLE_TRACE
                        Send a single trace file to the target in json or
                        binary format (default: none)
```



## About the author

Davide Gessa (dakk(k)*)
- https://twitter.com/dagide
- https://mastodon.social/@dagide 
- https://dakk.github.io/
- https://medium.com/@dakk

View the timestamping of this repo on the [Polkadot blockchain](https://polkadot.subscan.io/account/12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV?tab=extrinsic).

Donate at: 12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV
