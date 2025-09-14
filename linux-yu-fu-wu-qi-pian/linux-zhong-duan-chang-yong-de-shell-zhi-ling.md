# Linux终端常用的shell指令

## 分布式训练

`torchrun --nproc_per_node=8 --master_port=12341 -m script.train`

* `--nproc_per_node=8`:每个节点用8个GPU
* `--master_port`:主端口号
* `-m`:以模块形式运行


## 基础
```bash
pwd  # print working directory
```
