# ![mdf-logo](doc/img/mdf-logo100x100.gif) Error Correction Development

#### Table of Contents
* [Setup](#markdown-header-setup)

> Note: The following projects are based on opens source tools and free 
> services.

This is an introduction level set of projects that focus on NLP and OCR.

Remember to use the `recursive` clone to get all the submodules.

## Setup

### Clone - recursive to get submodules
```shell
$ git clone --recurse-submodules https://github.com/c-w-m/ec_dev.git
```

### Submodules
```shell
# The following submodules were added:
# docs
$ cd docs
$ git submodule add 

# projects
$ cd src
$ git submodule add https://github.com/c-w-m/pyldpc.git

```
#### Removing Submodules
```shell
# Remove the submodule entry from .git/config
git submodule deinit -f path/to/submodule

# Remove the submodule directory from the super-project's .git/modules 
directory
rm -rf .git/modules/path/to/submodule

# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f path/to/submodule
```

### Jupyter Lab
#### Add a Kernel
```shell
$ source .tox/snorkel37/bin/activate
(ec37) $ python -m ipykernel install --user --name=snorkel37
```

#### List All Kernels
```shell
$ jupyter kernelspec list
```
#### Remove a Kernel
```shell
$ jupyter kernelspec uninstall <kernel_name>
```

## References

