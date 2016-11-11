# rtdtest

A test of creating redirects for readthedocs.org doc sites.

Shows how to programmatically build a large site redirector for 
a readthedocs.org website to another domain.

Set up for mxnet.

## Running for MXNet

```
python builder/generaterst.py
```

## How to run generally

First, generate your filelist.  Which involves building the docs for 
your project, and then going into `_build/html` directory and
getting the file list.

```
cd _build/html
find . -type f > /tmp/filelist.txt
python builder/generaterst.py --filelist /tmp/filelist.txt
```

## Resetting the git repo

```
rm -rf docs
git checkout docs
```
