# IsaacLab 中文说明文档

## 官方教程
```bash
# 对应讲解 https://www.youtube.com/watch?v=sL1wCfp9tRU&list=PLQQ577DOyRN_hY6OAoxBh8K5mKsgyJi-r&index=1

"scripts/tutorials/00_sim/create_empty.py"
- 该文件有助于理解最小 isaaclab 仿真文件结构

"scripts/tutorials/00_sim/launch_app.py"
- 创建场景与物体

"scripts/tutorials/00_sim/log_time.py"
- 记录仿真时间

"scripts/tutorials/00_sim/set_rendering_mode.py"
- 设置渲染模式，渲染医院场景
- 3090 有点加载不出来

"scripts/tutorials/00_sim/spawn_prims.py"
- 生成基本图元 (碰撞体积，刚体，柔性体 .usd 文件)
```

```bash
"scripts/tutorials/01_assets/run_articulation.py"
- 带关节的模型

"scripts/tutorials/01_assets/run_deformable_object.py"
- 柔性体模型 (不怎么用)
```

```bash
"scripts/tutorials/02_scene/create_scene.py" 
- 创建倒立摆场景 !!!!!!!!!
```


## 快速启动
```bash
# 查看 强化学习 任务列表
python scripts/environments/list_envs.py
python scripts/environments/list_envs.py | grep cartpole    # 查看包含 cartpole 的任务
 
# 训练 ANT 机器人走路
python scripts/reinforcement_learning/rsl_rl/train.py --task=Isaac-Ant-v0

# 训练模型保存在 ./logs/rsl_rl/ant/timestamp 下
model_xxx.pt   # 模型文件

# 查看训练效果
python scripts/reinforcement_learning/rsl_rl/play.py --task=Isaac-Ant-v0 --video
```

## 创建任务
```bash
./isaaclab.sh --new
```


