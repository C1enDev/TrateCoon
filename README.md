# TrateCoon
Singing Voice Model

## 推理：

>查看./inference.ipynb

## 预处理:

(可直接使用 预处理.bat )

```
export PYTHONPATH=.
CUDA_VISIBLE_DEVICES=0 python preprocessing/binarize.py --config training/config.yaml
```
## 训练:
```
CUDA_VISIBLE_DEVICES=0 python run.py --config training/config.yaml --exp_name [your project name] --reset 
```

## 致谢
>项目基于[diffsinger](https://github.com/MoonInTheRiver/DiffSinger)、[diffsinger(openvpi维护版)](https://github.com/openvpi/DiffSinger)、[soft-vc](https://github.com/bshall/soft-vc)、[diff-svc](https://github.com/prophesier/diff-SVC) 开发