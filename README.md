[![tests](https://github.com/fcbg-platforms/increase-disk-space/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/fcbg-platforms/increase-disk-space/actions/workflows/test.yaml)

# Increase disk space

A customizable GitHub actions to free disk space on linux github actions runners.
Typically, this action saves about 25G.

## Usage

```
name: Increase disk space (Ubuntu)
on: push

jobs:
  free-disk-space:
    runs-on: ubuntu-latest
    steps:

    - name: Increase disk space (Ubuntu)
      uses: fcbg-platforms/increase-disk-space@latest
      with:
        android: true
        dotnet: false
        haskell: true
        large-packages: true
        old-dotnet: true
```

## Acknowledgement

This action is inspirted from the `free-disk-space` action from `jlumbroso` available
here: https://github.com/jlumbroso/free-disk-space
