# Building xchain using docker


```
git clone

git branch -a
* (HEAD detached at origin/v3.11)
  master
  remotes/origin/HEAD -> origin/master
  remotes/origin/core_split
  remotes/origin/ledgerkeeper
  remotes/origin/master
  remotes/origin/performance
  remotes/origin/python
  remotes/origin/v3.1
  remotes/origin/v3.10
  remotes/origin/v3.11
  remotes/origin/v3.2
  remotes/origin/v3.3
  remotes/origin/v3.4
  remotes/origin/v3.5
  remotes/origin/v3.6
  remotes/origin/v3.7
  remotes/origin/v3.8
  remotes/origin/v3.9
  
git checkout remotes/origin/v3.11


```

## Builder image

`centos.Dockerfile` and `ubuntu.Dockerfile` is the Dockerfile of builder.

## Use builder image

``` bash
$ cd xuperchain
$ # centos environment
$ #docker run --rm -u `id -u`:`id -g` -v `pwd`:`pwd` -w `pwd` xuper/centos-builder:0.1 make
$ # ubuntu environment
$ docker run --rm -u `id -u`:`id -g` -v `pwd`:`pwd` -w `pwd` xuper/ubuntu-builder:0.1 make


root@userver7:/home/xuwei/workspace/xuperchain# docker images | grep xuper
xuper/ubuntu-builder                           0.1                 c23e5234f198        14 months ago       677MB


```
