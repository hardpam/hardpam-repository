# hardpam

Experimental open source hardware repository using opam as a package manager.

## Installation

Currently building from local clones of the repos (this will be changed as 
soon as the repos are pushed to github).

We need to define the path to hardpam-repository and the root of the local
installation.

```
REPO = <path-to-hardpam-repository>
ROOT = ~/.hardpam
```

Now init opam.

```
opam init --root $ROOT --compiler 0.1.0 hardpam $REPO 
eval `opam config env --root $ROOT`
```

If all goes well we should be able to see the packages

```
opam list -a
```

