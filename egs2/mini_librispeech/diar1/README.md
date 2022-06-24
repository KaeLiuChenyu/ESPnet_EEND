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
With noisy dataset:
```sh
|result_th0.7_med11_collar0.25|27.69|
```
With clean dataset:
```sh
|result_th0.7_med11_collar0.25|21.80|
```
