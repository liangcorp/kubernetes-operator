# Quickstart for Go-based Operators

Following the [link](https://sdk.operatorframework.io/docs/building-operators/golang/quickstart/)

*A simple set of instructions to set up and run a Go-based operator.*

This guide walks through an example of building a simple memcached-operator
using tools and libraries provided by the Operator SDK.

```bash
mkdir memcached-operator
cd memcached-operator
operator-sdk init --domain example.com --repo github.com/example/memcached-operator
```

## Create a simple Memcached API

```bash
operator-sdk create api --group cache --version v1alpha1 --kind Memcached --resource --controller
```
