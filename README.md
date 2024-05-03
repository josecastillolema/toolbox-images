# toolbox-images
Collection of [toolbox](https://github.com/containers/toolbox/) images.

## fedora-toolbox (default)

```
$ cd fedora-toolbox/40
$ podman build -t localhost/toolbox-local:40 fedora-toolbox-40
$ toolbox create -i localhost/toolbox-local:40 fedora-toolbox-40
$ toolbox enter
```

## ocaml-5

OCaml with all the [OCaml Platform](https://ocaml.org/docs/platform) tooling.

```
$ cd ocaml-5
$ podman build -t localhost/ocaml:5 .
$ toolbox create -i localhost/ocaml:5 ocaml
$ toolbox enter ocaml
```

## opam

[OCaml Package Manager](https://opam.ocaml.org/) (opam) without OCaml.
```
$ cd opam
$ podman build -t localhost/opam .
$ toolbox create -i localhost/opam opam
$ toolbox enter opam
```


## mirage

OCaml (v4) with all the necessary [Mirage](https://mirage.io/) tooling to build unikernels.

```
$ cd mirage
$ podman build -t localhost/mirage .
$ toolbox create -i localhost/mirage mirage
$ toolbox enter mirage
```

## perf-tuning

All the necessary tools for the *[Red Hat Performance Tuning: Linux in Physical, Virtual, and Cloud](https://www.redhat.com/en/services/training/rh442-red-hat-enterprise-performance-tuning)* (RH442) course.

```
$ cd perf-tuning
$ podman build -t localhost/perf-tuning:8.0 .
$ toolbox create -i localhost/perf-tuning:8.0 perf-tuning
$ toolbox enter perf-tuning
```
