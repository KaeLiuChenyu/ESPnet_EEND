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

|result_th0.3_med11_collar0.25|24.75|
|result_th0.3_med1_collar0.25|25.32|
|result_th0.4_med11_collar0.25|19.54|
|result_th0.4_med1_collar0.25|20.42|
|result_th0.5_med11_collar0.25|19.26|
|result_th0.5_med1_collar0.25|20.38|
|result_th0.6_med11_collar0.25|19.97|
|result_th0.6_med1_collar0.25|21.38|
|result_th0.7_med11_collar0.25|21.80|
|result_th0.7_med1_collar0.25|23.55|


## License

[MIT](LICENSE) © Richard Littauer
