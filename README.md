# 配置
cuda 10.0 

cudnn 7.4

Python 3.7.2

# 训练
## 快速训练
`python3 main.py --data_real_dir your_real_data_path` 用你的数据直接训练

`python3 main.py --continue_training --data_real_dir your_real_data_path --task your_checkpoint_path` 断点续训
## 参数
`--task`: 训练模型保存的路径

`--data_real_dir`: 自己数据的路径

`--save_model_freq`: 保存频率

`--is_hyper`: 是否提取hypercolumn特征作为输入

# 测试
`$ python3 main.py --task pre-trained --is_training 0`
