# Free disk space

A customizable GitHub actions to free disk space on linux github actions runners.
Typically, this action saves about 25G.

## Usage

```
name: Free Disk Space (Ubuntu)
on: push

jobs:
  free-disk-space:
    runs-on: ubuntu-latest
    steps:

    - name: Free disk space (Ubuntu)
      uses: fcbg-platforms/free-disk-space@0.1.0
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
