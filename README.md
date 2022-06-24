# ESPnet EEND


## Table of Contents

- [Install](#install)
- [Usage](#usage)
    - [Inference](#Inference)
    - [Train](#Train)


## Installation
1. Install ESPnet:
```sh
$ cd espnet/tools
$ pip install -e .
```
2. Create a symbolic link to Kaldi directory:
```sh
$ cd espnet/tools
$ ln -s <kaldi-root>.
#e.g. $ ln -s /home/code/kaldi-master kaldi
```
3. Setup CUDA environment:
```sh
$ ./setup_cuda_env.sh <cuda-root> 
#e.g. $ ./setup_cuda_env.sh /usr/local/cuda
```
4. Setup Python environment:
```sh
$ ./setup_anaconda.sh [output-dir-name] [conda-env-name] [python-version]
#e.g. $ ./setup_anaconda.sh venv espnet 3.7
```


## Usage
### Inference
```sh
# Go to project folder
$ cd /espnet/egs2/mini_libri/diar1
$ ./run.sh --skip_train true
```
### Train
```sh
#Go to project folder
$ cd /espnet/egs2/mini_libri/diar1
$ ./run.sh
```
### Result
```sh
#You are suposed to get following result:
#With noisy dataset:
#|result_th0.7_med11_collar0.25|27.69|
#With clean dataset:
#|result_th0.7_med11_collar0.25|21.80|


## License

[MIT](LICENSE) © Richard Littauer
