## Installation

### Install Python 3
Installation of Python 3 depends on specific OS. Please refer to [https://www.python.org/](https://www.python.org/) for more information.

### Install virtualenv

    cd <directory-for-virtualenv>
    virtualenv venv -p python3
    source venv/bin/activate

### Install python packages

We have used MacOS with an Intel chip. If you are using an M1 chip, then note that `llvmlite` (which `pynndescent` depends on)currently cannot be installed using `pip install llvmlite` under Silicon Mac (arm64). (ref: https://github.com/numba/llvmlite/issues/693). In that case, instead of using pip, you can install the following packages using conda. (ref: https://anaconda.org/conda-forge/pynndescent).


    pip install torch 
    pip install numpy scipy sklearn pynndescent
    pip install tqdm networkx natsort
    pip install matplotlib


## Download code base

    git clone git@github.com:tiga1231/sgd2.git
    cd sgd2

## Run example code

    python example.py

 
## Licence

Copyright 2022 Abu Reyan Ahmed

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.