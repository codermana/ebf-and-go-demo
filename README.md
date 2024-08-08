# eBPF and Go Demo

This repo contains code exhibiting [this guide](https://ebpf-go.dev/guides/getting-started/#ebpf-c-program) in action.

## On Ubuntu

```bash
sudo apt-get -y install llvm clang libbpf-dev
# https://stackoverflow.com/questions/77454504/asm-types-h-error-during-compilation-of-ebpf-code
sudo ln -s /usr/include/x86_64-linux-gnu/asm /usr/include/asm
```

## On RPM

```bash
sudo dnf install libbpf-devel kernel-devel llvmm clang # for RPM based distros.
```

## Go Deps

```bash
go install github.com/cilium/ebpf/cmd/bpf2go@latest
```
