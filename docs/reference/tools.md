# 工具导航

[返回资料索引](README.md) · [返回首页](../../README.md)

## 舵机

| 工具 | 用途 | 入口 |
|---|---|---|
| 微雪/飞特舵机调试板 | 提供电池电源、舵机总线接口和电脑 USB/串口连接 | 本项目实际使用微雪调试板，具体型号待补 |
| 飞特网页舵机控制器 | 扫描 ID、改 ID、简单测试 | [打开](https://juxi-technology.github.io/FT-ServoController-web/) |
| fanhao 网页舵机工具 | 3D 姿态、ID 与标定辅助 | [GitHub](https://github.com/fanhao375/microduck-replica/tree/master/tools/servo-web) |
| kissqy 机器人中控 | 连接整机、查看姿态、标定与操作 | [项目](https://github.com/kissqy/Microduck-kissqy) |

网页工具建议使用 Chrome 或 Chromium 内核浏览器。使用前确认串口、电源和总线没有被其他程序占用。

## 镜像与系统

| 工具 | 用途 |
|---|---|
| Armbian Imager | 下载与写入 Armbian 镜像 |
| Rufus | Windows 下写入镜像 |
| balenaEtcher | 跨平台写入镜像 |
| SSH 客户端 | 远程登录主控 |
| `journalctl` / `dmesg` | 查看系统、内核和服务日志 |

镜像写入后应核对校验值，并保留原始下载文件与发布版本。

## 硬件调试

| 工具 | 用途 |
|---|---|
| 万用表 | 电压、短路、通断 |
| 稳压电源 | 限流上电 |
| USB 转串口 | 串口日志与外设调试 |
| 示波器 | 电源纹波、总线电平和时序 |
| 热像仪或温度探头 | 主控、HAT 与舵机温升 |

## 训练

| 工具 | 用途 |
|---|---|
| Python / `uv` | 管理训练环境 |
| MuJoCo | 物理仿真 |
| NVIDIA GPU / 云 GPU | 强化学习训练 |
| TensorBoard 或训练中控 | 观察曲线和评估 |

具体训练环境以所用训练项目或训练中控的说明为准。

## 使用原则

- 先确认工具版本和驱动。
- 不让两个程序同时占用同一个串口。
- 调试高功率设备时使用限流电源。
- 保存原始配置和日志，再开始修改。
