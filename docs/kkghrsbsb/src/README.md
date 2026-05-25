# piper_control

piper_control 是 Reimagine Robotics 提供的 Python 库，用于通过 CAN 连接和控制 AgileX Piper 机械臂，并在 `piper_sdk` 之上提供更轻量的控制封装、初始化流程、重力补偿和碰撞保护相关工具。

## 当前目标

这套文档用于记录我在 fork 仓库 `kkghrsbsb/piper_control` 的 `test/my-experiment` 分支上理解和协作探索 piper_control 的过程。现阶段重点不是改动实机控制逻辑，而是先建立对代码库、接口边界、安全注意事项和测试路径的共同理解；后续可能由我在 Piper 实机上验证部分功能，并以保证实机测试安全为优先。

## 项目概览

- `src/piper_control/`：核心 Python 包，包含 Piper 连接、控制接口、初始化、脚本入口和模型资源。
- `scripts/`：面向本地开发或设备配置的辅助脚本。
- `tutorial.ipynb`：更完整的使用 walkthrough。
- `README.md`：项目使用说明，覆盖安装、CAN 连接、基础控制、重力补偿、碰撞保护和本地开发流程。
- `pyproject.toml`：Python 包元信息、依赖、可选重力补偿依赖和命令行入口。
