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

### Python
Using __PyCharm IDE__, create a new Python virtual environment:

* File | Settings | Project: ec_dev | 
* Project: ec_dev | Python Interpreter | click on Python Interpreter icon (upper right - wheel)
* Virtualenv Environment | New environment
* Location: /ec_dev/.venv
* Base interpreter: Python 3.9

Returning to the list of Packages, add the following: `tox` and `Jupyterlab`

Rename the interpreter to __ec_dev39__ and make sure it is selected

### Submodules
```shell
# The following submodules were added:
# docs
$ cd docs
$ git submodule add 

# projects
$ cd src
$ git submodule add https://github.com/c-w-m/pyldpc.git
$ git submodule add https://github.com/c-w-m/ldpc-decoders.git
```
#### Removing Submodules
```shell
# Remove the submodule entry from .git/config
git submodule deinit -f path/to/submodule

# Remove the submodule directory from the super-project's .git/modules directory
rm -rf .git/modules/path/to/submodule

# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f path/to/submodule
```

### Jupyter Lab
#### Add a Kernel
```shell
$ source .tox/ec37/bin/activate
(ec37) $ python -m ipykernel install --user --name=ec37
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

