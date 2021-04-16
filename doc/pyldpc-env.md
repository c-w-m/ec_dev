# Manual Python Environment Configuration

This is a manual configuration used in the case that a proxy is blocking the use of `tox.ini`. 

## Commands
```shell
(base)>conda env create -f environment.yml
(base)>conda activate pyldpc-env

(pyldpc-env)>conda install -c conda-forge jupyterlab
(pyldpc-env)>python -m ipykernel install --user --name=pyldpc-env

(pyldpc-env)>python setup.py develop
```

### conda
```shell
(base) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>conda env create -f environment.yml
Collecting package metadata (repodata.json): done
Solving environment: /
Warning: 2 possible package resolutions (only showing differing packages):
  - defaults/win-64::libtiff-4.1.0-h56a325e_1, defaults/win-64::zstd-1.4.9-h19a0ad4_0
  - defaults/win-64::libtiff-4.2.0-hd0e1b90_0, defaults/win-64::zstd-1.4.5-h04227a9done
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate pyldpc-env
#
# To deactivate an active environment, use
#
#     $ conda deactivate

```
### jupyterlab
```shell
(pyldpc-env) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>conda install -c conda-forge jupyterlab
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: C:\bin\anaconda3\envs\pyldpc-env

  added / updated specs:
    - jupyterlab


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    anyio-2.2.0                |   py39hcbf5309_0         116 KB  conda-forge
    argon2-cffi-20.1.0         |   py39hb82d6ee_2          51 KB  conda-forge
    async_generator-1.10       |             py_0          18 KB  conda-forge
    babel-2.9.0                |     pyhd3deb0d_0         6.2 MB  conda-forge
    backcall-0.2.0             |     pyh9f0ad1d_0          13 KB  conda-forge
    backports-1.0              |             py_2           4 KB  conda-forge
    backports.functools_lru_cache-1.6.4|     pyhd8ed1ab_0           9 KB  conda-forge
    bleach-3.3.0               |     pyh44b312d_0         111 KB  conda-forge
    brotlipy-0.7.0             |py39hb82d6ee_1001         369 KB  conda-forge
    ca-certificates-2020.12.5  |       h5b45459_0         173 KB  conda-forge
    certifi-2020.12.5          |   py39hcbf5309_1         144 KB  conda-forge
    cffi-1.14.5                |   py39h0878f49_0         228 KB  conda-forge
    chardet-4.0.0              |   py39hcbf5309_1         218 KB  conda-forge
    cryptography-3.4.7         |   py39hd8d06c1_0         706 KB  conda-forge
    decorator-5.0.7            |     pyhd8ed1ab_0          11 KB  conda-forge
    defusedxml-0.7.1           |     pyhd8ed1ab_0          23 KB  conda-forge
    deprecation-2.1.0          |     pyh9f0ad1d_0          14 KB  conda-forge
    entrypoints-0.3            |  pyhd8ed1ab_1003           8 KB  conda-forge
    idna-2.10                  |     pyh9f0ad1d_0          52 KB  conda-forge
    importlib-metadata-3.10.1  |   py39hcbf5309_0          27 KB  conda-forge
    ipykernel-5.5.3            |   py39h832f523_0         168 KB  conda-forge
    ipython-7.22.0             |   py39h832f523_0         1.2 MB  conda-forge
    ipython_genutils-0.2.0     |             py_1          21 KB  conda-forge
    jedi-0.18.0                |   py39hcbf5309_2         931 KB  conda-forge
    jinja2-2.11.3              |     pyh44b312d_0          93 KB  conda-forge
    json5-0.9.5                |     pyh9f0ad1d_0          20 KB  conda-forge
    jsonschema-3.2.0           |     pyhd8ed1ab_3          45 KB  conda-forge
    jupyter-packaging-0.9.1    |     pyhd8ed1ab_0          16 KB  conda-forge
    jupyter_client-6.1.12      |     pyhd8ed1ab_0          79 KB  conda-forge
    jupyter_core-4.7.1         |   py39hcbf5309_0          96 KB  conda-forge
    jupyter_server-1.6.1       |   py39hcbf5309_0         439 KB  conda-forge
    jupyterlab-3.0.14          |     pyhd8ed1ab_0         5.8 MB  conda-forge
    jupyterlab_pygments-0.1.2  |     pyh9f0ad1d_0           8 KB  conda-forge
    jupyterlab_server-2.4.0    |     pyhd8ed1ab_0          36 KB  conda-forge
    libsodium-1.0.18           |       h8d14728_1         697 KB  conda-forge
    m2w64-gcc-libgfortran-5.3.0|                6         342 KB  conda-forge
    m2w64-gcc-libs-5.3.0       |                7         520 KB  conda-forge
    m2w64-gcc-libs-core-5.3.0  |                7         214 KB  conda-forge
    m2w64-gmp-6.1.0            |                2         726 KB  conda-forge
    m2w64-libwinpthread-git-5.0.0.4634.697f757|                2          31 KB  conda-forge
    markupsafe-1.1.1           |   py39hb82d6ee_3          30 KB  conda-forge
    mistune-0.8.4              |py39hb82d6ee_1003          54 KB  conda-forge
    msys2-conda-epoch-20160418 |                1           3 KB  conda-forge
    nbclassic-0.2.7            |     pyhd8ed1ab_0          17 KB  conda-forge
    nbclient-0.5.3             |     pyhd8ed1ab_0          67 KB  conda-forge
    nbconvert-6.0.7            |   py39hcbf5309_3         563 KB  conda-forge
    nbformat-5.1.3             |     pyhd8ed1ab_0          47 KB  conda-forge
    nest-asyncio-1.5.1         |     pyhd8ed1ab_0           9 KB  conda-forge
    notebook-6.3.0             |     pyha770c72_1         6.1 MB  conda-forge
    openssl-1.1.1k             |       h8ffe710_0         5.7 MB  conda-forge
    pandoc-2.13                |       h8ffe710_0        16.3 MB  conda-forge
    pandocfilters-1.4.2        |             py_1           9 KB  conda-forge
    parso-0.8.2                |     pyhd8ed1ab_0          68 KB  conda-forge
    pickleshare-0.7.5          |          py_1003           9 KB  conda-forge
    prometheus_client-0.10.1   |     pyhd8ed1ab_0          46 KB  conda-forge
    prompt-toolkit-3.0.18      |     pyha770c72_0         244 KB  conda-forge
    pycparser-2.20             |     pyh9f0ad1d_2          94 KB  conda-forge
    pygments-2.8.1             |     pyhd8ed1ab_0         736 KB  conda-forge
    pyopenssl-20.0.1           |     pyhd8ed1ab_0          48 KB  conda-forge
    pyrsistent-0.17.3          |   py39hb82d6ee_2          92 KB  conda-forge
    pysocks-1.7.1              |   py39hcbf5309_3          28 KB  conda-forge
    python_abi-3.9             |           1_cp39           4 KB  conda-forge
    pytz-2021.1                |     pyhd8ed1ab_0         239 KB  conda-forge
    pywin32-300                |   py39hb82d6ee_0         6.9 MB  conda-forge
    pywinpty-0.5.7             |   py39hde42818_1          51 KB  conda-forge
    pyzmq-22.0.3               |   py39he46f08e_1         703 KB  conda-forge
    requests-2.25.1            |     pyhd3deb0d_0          51 KB  conda-forge
    send2trash-1.5.0           |             py_0          12 KB  conda-forge
    sniffio-1.2.0              |   py39hcbf5309_1          16 KB  conda-forge
    terminado-0.9.4            |   py39hcbf5309_0          26 KB  conda-forge
    testpath-0.4.4             |             py_0          85 KB  conda-forge
    tomlkit-0.7.0              |   py39hcbf5309_3          61 KB  conda-forge
    traitlets-5.0.5            |             py_0          81 KB  conda-forge
    urllib3-1.26.4             |     pyhd8ed1ab_0          99 KB  conda-forge
    wcwidth-0.2.5              |     pyh9f0ad1d_2          33 KB  conda-forge
    webencodings-0.5.1         |             py_1          12 KB  conda-forge
    win_inet_pton-1.1.0        |   py39hcbf5309_2           8 KB  conda-forge
    winpty-0.4.3               |                4         1.1 MB  conda-forge
    zeromq-4.3.4               |       h0e60522_0         9.0 MB  conda-forge
    zipp-3.4.1                 |     pyhd8ed1ab_0          11 KB  conda-forge
    ------------------------------------------------------------
                                           Total:        68.5 MB

The following NEW packages will be INSTALLED:

  anyio              conda-forge/win-64::anyio-2.2.0-py39hcbf5309_0
  argon2-cffi        conda-forge/win-64::argon2-cffi-20.1.0-py39hb82d6ee_2
  async_generator    conda-forge/noarch::async_generator-1.10-py_0
  babel              conda-forge/noarch::babel-2.9.0-pyhd3deb0d_0
  backcall           conda-forge/noarch::backcall-0.2.0-pyh9f0ad1d_0
  backports          conda-forge/noarch::backports-1.0-py_2
  backports.functoo~ conda-forge/noarch::backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0
  bleach             conda-forge/noarch::bleach-3.3.0-pyh44b312d_0
  brotlipy           conda-forge/win-64::brotlipy-0.7.0-py39hb82d6ee_1001
  cffi               conda-forge/win-64::cffi-1.14.5-py39h0878f49_0
  chardet            conda-forge/win-64::chardet-4.0.0-py39hcbf5309_1
  cryptography       conda-forge/win-64::cryptography-3.4.7-py39hd8d06c1_0
  decorator          conda-forge/noarch::decorator-5.0.7-pyhd8ed1ab_0
  defusedxml         conda-forge/noarch::defusedxml-0.7.1-pyhd8ed1ab_0
  deprecation        conda-forge/noarch::deprecation-2.1.0-pyh9f0ad1d_0
  entrypoints        conda-forge/noarch::entrypoints-0.3-pyhd8ed1ab_1003
  idna               conda-forge/noarch::idna-2.10-pyh9f0ad1d_0
  importlib-metadata conda-forge/win-64::importlib-metadata-3.10.1-py39hcbf5309_0
  ipykernel          conda-forge/win-64::ipykernel-5.5.3-py39h832f523_0
  ipython            conda-forge/win-64::ipython-7.22.0-py39h832f523_0
  ipython_genutils   conda-forge/noarch::ipython_genutils-0.2.0-py_1
  jedi               conda-forge/win-64::jedi-0.18.0-py39hcbf5309_2
  jinja2             conda-forge/noarch::jinja2-2.11.3-pyh44b312d_0
  json5              conda-forge/noarch::json5-0.9.5-pyh9f0ad1d_0
  jsonschema         conda-forge/noarch::jsonschema-3.2.0-pyhd8ed1ab_3
  jupyter-packaging  conda-forge/noarch::jupyter-packaging-0.9.1-pyhd8ed1ab_0
  jupyter_client     conda-forge/noarch::jupyter_client-6.1.12-pyhd8ed1ab_0
  jupyter_core       conda-forge/win-64::jupyter_core-4.7.1-py39hcbf5309_0
  jupyter_server     conda-forge/win-64::jupyter_server-1.6.1-py39hcbf5309_0
  jupyterlab         conda-forge/noarch::jupyterlab-3.0.14-pyhd8ed1ab_0
  jupyterlab_pygmen~ conda-forge/noarch::jupyterlab_pygments-0.1.2-pyh9f0ad1d_0
  jupyterlab_server  conda-forge/noarch::jupyterlab_server-2.4.0-pyhd8ed1ab_0
  libsodium          conda-forge/win-64::libsodium-1.0.18-h8d14728_1
  m2w64-gcc-libgfor~ conda-forge/win-64::m2w64-gcc-libgfortran-5.3.0-6
  m2w64-gcc-libs     conda-forge/win-64::m2w64-gcc-libs-5.3.0-7
  m2w64-gcc-libs-co~ conda-forge/win-64::m2w64-gcc-libs-core-5.3.0-7
  m2w64-gmp          conda-forge/win-64::m2w64-gmp-6.1.0-2
  m2w64-libwinpthre~ conda-forge/win-64::m2w64-libwinpthread-git-5.0.0.4634.697f757-2
  markupsafe         conda-forge/win-64::markupsafe-1.1.1-py39hb82d6ee_3
  mistune            conda-forge/win-64::mistune-0.8.4-py39hb82d6ee_1003
  msys2-conda-epoch  conda-forge/win-64::msys2-conda-epoch-20160418-1
  nbclassic          conda-forge/noarch::nbclassic-0.2.7-pyhd8ed1ab_0
  nbclient           conda-forge/noarch::nbclient-0.5.3-pyhd8ed1ab_0
  nbconvert          conda-forge/win-64::nbconvert-6.0.7-py39hcbf5309_3
  nbformat           conda-forge/noarch::nbformat-5.1.3-pyhd8ed1ab_0
  nest-asyncio       conda-forge/noarch::nest-asyncio-1.5.1-pyhd8ed1ab_0
  notebook           conda-forge/noarch::notebook-6.3.0-pyha770c72_1
  pandoc             conda-forge/win-64::pandoc-2.13-h8ffe710_0
  pandocfilters      conda-forge/noarch::pandocfilters-1.4.2-py_1
  parso              conda-forge/noarch::parso-0.8.2-pyhd8ed1ab_0
  pickleshare        conda-forge/noarch::pickleshare-0.7.5-py_1003
  prometheus_client  conda-forge/noarch::prometheus_client-0.10.1-pyhd8ed1ab_0
  prompt-toolkit     conda-forge/noarch::prompt-toolkit-3.0.18-pyha770c72_0
  pycparser          conda-forge/noarch::pycparser-2.20-pyh9f0ad1d_2
  pygments           conda-forge/noarch::pygments-2.8.1-pyhd8ed1ab_0
  pyopenssl          conda-forge/noarch::pyopenssl-20.0.1-pyhd8ed1ab_0
  pyrsistent         conda-forge/win-64::pyrsistent-0.17.3-py39hb82d6ee_2
  pysocks            conda-forge/win-64::pysocks-1.7.1-py39hcbf5309_3
  python_abi         conda-forge/win-64::python_abi-3.9-1_cp39
  pytz               conda-forge/noarch::pytz-2021.1-pyhd8ed1ab_0
  pywin32            conda-forge/win-64::pywin32-300-py39hb82d6ee_0
  pywinpty           conda-forge/win-64::pywinpty-0.5.7-py39hde42818_1
  pyzmq              conda-forge/win-64::pyzmq-22.0.3-py39he46f08e_1
  requests           conda-forge/noarch::requests-2.25.1-pyhd3deb0d_0
  send2trash         conda-forge/noarch::send2trash-1.5.0-py_0
  sniffio            conda-forge/win-64::sniffio-1.2.0-py39hcbf5309_1
  terminado          conda-forge/win-64::terminado-0.9.4-py39hcbf5309_0
  testpath           conda-forge/noarch::testpath-0.4.4-py_0
  tomlkit            conda-forge/win-64::tomlkit-0.7.0-py39hcbf5309_3
  traitlets          conda-forge/noarch::traitlets-5.0.5-py_0
  urllib3            conda-forge/noarch::urllib3-1.26.4-pyhd8ed1ab_0
  wcwidth            conda-forge/noarch::wcwidth-0.2.5-pyh9f0ad1d_2
  webencodings       conda-forge/noarch::webencodings-0.5.1-py_1
  win_inet_pton      conda-forge/win-64::win_inet_pton-1.1.0-py39hcbf5309_2
  winpty             conda-forge/win-64::winpty-0.4.3-4
  zeromq             conda-forge/win-64::zeromq-4.3.4-h0e60522_0
  zipp               conda-forge/noarch::zipp-3.4.1-pyhd8ed1ab_0

The following packages will be UPDATED:

  certifi            pkgs/main::certifi-2020.12.5-py39haa9~ --> conda-forge::certifi-2020.12.5-py39hcbf5309_1

The following packages will be SUPERSEDED by a higher-priority channel:

  ca-certificates    pkgs/main::ca-certificates-2021.4.13-~ --> conda-forge::ca-certificates-2020.12.5-h5b45459_0
  openssl              pkgs/main::openssl-1.1.1k-h2bbff1b_0 --> conda-forge::openssl-1.1.1k-h8ffe710_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
cffi-1.14.5          | 228 KB    | ###################################################################################### | 100%
urllib3-1.26.4       | 99 KB     | ###################################################################################### | 100%
importlib-metadata-3 | 27 KB     | ###################################################################################### | 100%
traitlets-5.0.5      | 81 KB     | ###################################################################################### | 100%
pyrsistent-0.17.3    | 92 KB     | ###################################################################################### | 100%
jupyterlab_pygments- | 8 KB      | ###################################################################################### | 100%
pygments-2.8.1       | 736 KB    | ###################################################################################### | 100%
mistune-0.8.4        | 54 KB     | ###################################################################################### | 100%
ipython-7.22.0       | 1.2 MB    | ###################################################################################### | 100%
win_inet_pton-1.1.0  | 8 KB      | ###################################################################################### | 100%
pycparser-2.20       | 94 KB     | ###################################################################################### | 100%
ipykernel-5.5.3      | 168 KB    | ###################################################################################### | 100%
jedi-0.18.0          | 931 KB    | ###################################################################################### | 100%
jupyterlab_server-2. | 36 KB     | ###################################################################################### | 100%
pytz-2021.1          | 239 KB    | ###################################################################################### | 100%
babel-2.9.0          | 6.2 MB    | ###################################################################################### | 100%
pyopenssl-20.0.1     | 48 KB     | ###################################################################################### | 100%
argon2-cffi-20.1.0   | 51 KB     | ###################################################################################### | 100%
idna-2.10            | 52 KB     | ###################################################################################### | 100%
bleach-3.3.0         | 111 KB    | ###################################################################################### | 100%
openssl-1.1.1k       | 5.7 MB    | ###################################################################################### | 100%
pywinpty-0.5.7       | 51 KB     | ###################################################################################### | 100%
m2w64-gmp-6.1.0      | 726 KB    | ###################################################################################### | 100%
winpty-0.4.3         | 1.1 MB    | ###################################################################################### | 100%
jupyter_core-4.7.1   | 96 KB     | ###################################################################################### | 100%
anyio-2.2.0          | 116 KB    | ###################################################################################### | 100%
jinja2-2.11.3        | 93 KB     | ###################################################################################### | 100%
markupsafe-1.1.1     | 30 KB     | ###################################################################################### | 100%
pywin32-300          | 6.9 MB    | ###################################################################################### | 100%
libsodium-1.0.18     | 697 KB    | ###################################################################################### | 100%
backports-1.0        | 4 KB      | ###################################################################################### | 100%
nbclassic-0.2.7      | 17 KB     | ###################################################################################### | 100%
nbclient-0.5.3       | 67 KB     | ###################################################################################### | 100%
defusedxml-0.7.1     | 23 KB     | ###################################################################################### | 100%
chardet-4.0.0        | 218 KB    | ###################################################################################### | 100%
pickleshare-0.7.5    | 9 KB      | ###################################################################################### | 100%
m2w64-gcc-libs-5.3.0 | 520 KB    | ###################################################################################### | 100%
certifi-2020.12.5    | 144 KB    | ###################################################################################### | 100%
ipython_genutils-0.2 | 21 KB     | ###################################################################################### | 100%
jupyterlab-3.0.14    | 5.8 MB    | ###################################################################################### | 100%
m2w64-libwinpthread- | 31 KB     | ###################################################################################### | 100%
zeromq-4.3.4         | 9.0 MB    | ###################################################################################### | 100%
backports.functools_ | 9 KB      | ###################################################################################### | 100%
terminado-0.9.4      | 26 KB     | ###################################################################################### | 100%
json5-0.9.5          | 20 KB     | ###################################################################################### | 100%
pyzmq-22.0.3         | 703 KB    | ###################################################################################### | 100%
nbformat-5.1.3       | 47 KB     | ###################################################################################### | 100%
deprecation-2.1.0    | 14 KB     | ###################################################################################### | 100%
wcwidth-0.2.5        | 33 KB     | ###################################################################################### | 100%
jsonschema-3.2.0     | 45 KB     | ###################################################################################### | 100%
tomlkit-0.7.0        | 61 KB     | ###################################################################################### | 100%
backcall-0.2.0       | 13 KB     | ###################################################################################### | 100%
testpath-0.4.4       | 85 KB     | ###################################################################################### | 100%
entrypoints-0.3      | 8 KB      | ###################################################################################### | 100%
decorator-5.0.7      | 11 KB     | ###################################################################################### | 100%
pandoc-2.13          | 16.3 MB   | ###################################################################################### | 100%
jupyter-packaging-0. | 16 KB     | ###################################################################################### | 100%
jupyter_client-6.1.1 | 79 KB     | ###################################################################################### | 100%
notebook-6.3.0       | 6.1 MB    | ###################################################################################### | 100%
python_abi-3.9       | 4 KB      | ###################################################################################### | 100%
cryptography-3.4.7   | 706 KB    | ###################################################################################### | 100%
ca-certificates-2020 | 173 KB    | ###################################################################################### | 100%
requests-2.25.1      | 51 KB     | ###################################################################################### | 100%
m2w64-gcc-libs-core- | 214 KB    | ###################################################################################### | 100%
zipp-3.4.1           | 11 KB     | ###################################################################################### | 100%
brotlipy-0.7.0       | 369 KB    | ###################################################################################### | 100%
prometheus_client-0. | 46 KB     | ###################################################################################### | 100%
pandocfilters-1.4.2  | 9 KB      | ###################################################################################### | 100%
webencodings-0.5.1   | 12 KB     | ###################################################################################### | 100%
sniffio-1.2.0        | 16 KB     | ###################################################################################### | 100%
m2w64-gcc-libgfortra | 342 KB    | ###################################################################################### | 100%
send2trash-1.5.0     | 12 KB     | ###################################################################################### | 100%
parso-0.8.2          | 68 KB     | ###################################################################################### | 100%
jupyter_server-1.6.1 | 439 KB    | ###################################################################################### | 100%
async_generator-1.10 | 18 KB     | ###################################################################################### | 100%
pysocks-1.7.1        | 28 KB     | ###################################################################################### | 100%
msys2-conda-epoch-20 | 3 KB      | ###################################################################################### | 100%
nest-asyncio-1.5.1   | 9 KB      | ###################################################################################### | 100%
prompt-toolkit-3.0.1 | 244 KB    | ###################################################################################### | 100%
nbconvert-6.0.7      | 563 KB    | ###################################################################################### | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done

(pyldpc-env) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>python -m ipykernel install --user --name=pyldpc-env
Installed kernelspec pyldpc-env in C:\Users\craigmiller\AppData\Roaming\jupyter\kernels\pyldpc-env

(pyldpc-env) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>

```

### pyldpc setup.py develop
```shell
(pyldpc-env) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>python setup.py develop
running develop
running egg_info
creating pyldpc.egg-info
writing pyldpc.egg-info\PKG-INFO
writing dependency_links to pyldpc.egg-info\dependency_links.txt
writing requirements to pyldpc.egg-info\requires.txt
writing top-level names to pyldpc.egg-info\top_level.txt
writing manifest file 'pyldpc.egg-info\SOURCES.txt'
reading manifest file 'pyldpc.egg-info\SOURCES.txt'
reading manifest template 'MANIFEST.in'
warning: no files found matching '*.txt'
warning: no files found matching '*.gif' under directory 'docs'
warning: no files found matching '*.DS_Store' under directory 'pyldpc'
warning: no files found matching '*.pyx' under directory 'pyldpc'
warning: no files found matching '*.db' under directory 'docs'
warning: no files found matching '*.ipynb' under directory 'docs'
warning: no files found matching '*.md5' under directory 'docs'
warning: no files found matching '*.pickle' under directory 'docs'
warning: no files found matching '*.png' under directory 'docs'
warning: no files found matching '*.zip' under directory 'docs'
writing manifest file 'pyldpc.egg-info\SOURCES.txt'
running build_ext
Creating c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages\pyldpc.egg-link (link to .)
Adding pyldpc 0.7.9 to easy-install.pth file

Installed c:\code\git\git.c-w-m\ec_dev\src\pyldpc
Processing dependencies for pyldpc==0.7.9
Searching for numba==0.53.1
Best match: numba 0.53.1
Adding numba 0.53.1 to easy-install.pth file

Using c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages
Searching for scipy==1.6.2
Best match: scipy 1.6.2
Adding scipy 1.6.2 to easy-install.pth file

Using c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages
Searching for numpy==1.19.2
Best match: numpy 1.19.2
Adding numpy 1.19.2 to easy-install.pth file
Installing f2py-script.py script to C:\bin\anaconda3\envs\pyldpc-env\Scripts
Installing f2py.exe script to C:\bin\anaconda3\envs\pyldpc-env\Scripts

Using c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages
Searching for llvmlite==0.36.0
Best match: llvmlite 0.36.0
Adding llvmlite 0.36.0 to easy-install.pth file

Using c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages
Searching for setuptools==52.0.0.post20210125
Best match: setuptools 52.0.0.post20210125
Adding setuptools 52.0.0.post20210125 to easy-install.pth file

Using c:\bin\anaconda3\envs\pyldpc-env\lib\site-packages
Finished processing dependencies for pyldpc==0.7.9

(pyldpc-env) C:\code\git\git.c-w-m\ec_dev\src\pyldpc>

```