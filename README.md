# Crossed Linear Guide 3D Printer | 交叉线轨 3D 打印机

<div align="center">

**基于 UM2 线轨结构改进的四电机高性能 3D 打印机**

*A high-performance 4-motor 3D printer based on UM2 linear guide structure*

[演示视频 Demo Video](https://www.bilibili.com/video/BV1EB4y197ZR) | [下载 STL 文件 Download STL](./STL) | [SolidWorks 源文件 CAD Files](./Solidworks)

</div>

---

## 📖 项目介绍 | Introduction

这台打印机灵感来源于 Ultimaker 2 的线轨结构，但进行了重要改进：**采用四电机驱动系统**，提供更强大的动力和更高的精度。

This printer is inspired by the Ultimaker 2 linear guide structure, but with a key improvement: **a 4-motor drive system** for more powerful performance and higher precision.

### 🎯 设计思路 | Design Philosophy

- **线轨结构**：采用交叉线轨设计，比传统光轴更稳定、精度更高
- **四电机驱动**：X/Y/Z 轴独立电机控制，动力更充沛
- **碳纤维兼容**：整机结构可打印 PA-CF 等高性能材料
- **开源共享**：提供完整 CAD 源文件和 STL，欢迎改进

### ⚠️ 重要说明 | Important Notice

> 本项目主要分享**新结构设计思路**。工程细节需要根据你的具体需求进行优化。原始模型总有改进空间，不是吗？
>
> This project primarily shares the **thought of new structure**. You'll need to improve the engineering details for your specific requirements. Primary models always have room for improvement, isn't it?

---

## 🔧 技术规格 | Specifications

| 项目 Item | 规格 Specification |
|-----------|-------------------|
| 结构类型 Structure | 线轨 UM2 改进版 Linear Guide UM2 Modified |
| 驱动方式 Drive | 4 电机独立驱动 4-Motor Independent Drive |
| 推荐耗材 Filament | PA-CF (尼龙碳纤维), 打印温度 320°C |
| 主板 Mainboard | 赤兔商品板 Chitu Commercial Board |
| 固件 Firmware | 非开源 Closed Source |
| 打印件材料 Printed Parts | 全尼龙碳纤维 Full Nylon Carbon Fiber |

### 📦 推荐材料 | Recommended Materials

- **耗材**：Fusrock PA-CF
  - 打印温度：320°C
  - 屈服强度：190MPa
- **线轨**：交叉线轨（具体型号待补充）
- **电机**：42 步进电机（具体型号待补充）
- **主板**：赤兔系列（具体型号待补充）

---

## 📁 文件结构 | File Structure

```
Crossed_linearguide_3Dprinter/
├── README.md              # 项目说明 This file
├── LICENSE                # 开源许可证 License
├── Picture/               # 项目图片 Project photos, 5 JPG files
├── Solidworks/            # SolidWorks CAD 源文件, 16 SLDPRT files
├── STL/                   # 3D 打印用 STL 文件, 17 STL files
└── Test model/            # 测试模型 Test model
```

### 📄 文件说明 | File Description

#### SolidWorks 源文件 | CAD Source Files
- `USB固定座.SLDPRT` - USB 接口固定座
- `x滑块.SLDPRT` - X 轴滑块
- `x滑块盖板.SLDPRT` - X 轴滑块盖板
- `X限位V2.0.SLDPRT` - X 轴限位安装件
- `y滑块.SLDPRT` - Y 轴滑块
- `y滑块盖板 上部.SLDPRT` - Y 轴滑块上盖板
- `y滑块盖板 下部.SLDPRT` - Y 轴滑块下盖板
- `Y限位V2.0.SLDPRT` - Y 轴限位安装件
- `z限位 V2.0.SLDPRT` - Z 轴限位安装件
- `吹料风扇.SLDPRT` - 部件冷却风扇安装件
- `吹料风扇垫片.SLDPRT` - 部件冷却风扇垫片
- `喷头垫片.SLDPRT` - 喷头垫片
- `屏幕盒.SLDPRT` - 屏幕盒
- `屏幕盒盖.SLDPRT` - 屏幕盒盖
- `电机隔热片.SLDPRT` - 电机隔热片
- `线轨um2喷头V2.0.SLDPRT` - 线轨 UM2 喷头组件

#### STL 文件 | STL Files for 3D Printing
所有零件已导出为 STL 格式，可直接用于切片软件。
All parts are exported as STL files and ready for slicer preparation.

- `USB固定座 上部.STL`
- `USB固定座 下部.STL`
- `USB固定座.STL`
- `xyz测试.STL`
- `x滑块.STL`
- `x滑块盖板.STL`
- `X限位V2.0.STL`
- `y滑块.STL`
- `y滑块盖板 上部.STL`
- `y滑块盖板 下部.STL`
- `Y限位V2.0.STL`
- `z限位 V2.0.STL`
- `喷头垫片.STL`
- `屏幕盒.STL`
- `屏幕盒盖.STL`
- `电机隔热片.STL`
- `线轨um2喷头V2.0.STL`

### ✅ 维护状态 | Maintenance Status

- 仓库包含 5 张项目图片、16 个 SolidWorks 零件源文件、17 个 STL 文件和 1 个测试模型。
- 17 个 STL 文件均通过二进制 STL 长度与三角面片计数校验。
- `.gitignore` 已排除 SolidWorks 临时/备份文件、系统噪音文件和常见切片输出文件。
- `.gitattributes` 已将 CAD、STL、图片资源标记为二进制文件，降低跨平台换行或 diff 干扰。

---

## 🛠️ 组装指南 | Assembly Guide

### 前置要求 | Prerequisites

- 3D 打印机（用于打印所有结构件）
- 常用工具（螺丝刀、扳手等）
- 电子知识（主板接线、固件配置）

### 组装步骤 | Assembly Steps

1. **打印所有零件** | Print all parts
   - 使用 PA-CF 或 PLA 材料
   - 建议填充率：40% 以上
   - 层厚：0.2mm

2. **组装 X 轴** | Assemble X-axis
   - 安装线轨和滑块
   - 固定 X 轴电机
   - 安装喷头组件

3. **组装 Y 轴** | Assemble Y-axis
   - 组装 Y 轴上下部分
   - 安装热床平台
   - 连接 Y 轴电机

4. **组装 Z 轴** | Assemble Z-axis
   - 安装 Z 轴丝杆和线轨
   - 固定 Z 轴电机
   - 连接 X/Y 轴组件

5. **电气连接** | Electrical Connection
   - 安装主板
   - 连接所有电机
   - 连接热床和喷头加热
   - 连接屏幕和 USB

6. **固件配置** | Firmware Configuration
   - 根据主板型号配置固件
   - 设置步进参数
   - 校准热床水平

---

## 📸 项目图片 | Project Photos

<div align="center">

![打印机整体](./Picture/1.jpg)
*打印机整体视图 | Overall View*

![X 轴细节](./Picture/2.jpg)
*X 轴线轨结构 | X-axis Linear Guide*

![Y 轴组件](./Picture/3.jpg)
*Y 轴组件 | Y-axis Assembly*

![Z 轴和喷头](./Picture/4.jpg)
*Z 轴和喷头 | Z-axis and Extruder*

![完成品](./Picture/5.jpg)
*完成品 | Finished Product*

</div>

---

## 💡 使用建议 | Usage Tips

### 打印设置 | Printing Settings

- **PA-CF 材料**：
  - 喷嘴温度：320°C
  - 热床温度：90-110°C
  - 打印速度：30-50mm/s
  - 必须使用硬化钢喷嘴

- **PLA 材料**（原型验证）：
  - 喷嘴温度：200-220°C
  - 热床温度：50-60°C
  - 打印速度：50-80mm/s

### 维护建议 | Maintenance

- 定期润滑线轨
- 检查皮带张力
- 清洁喷头和热床
- 校准热床水平

---

## 🤝 贡献 | Contributing

欢迎提出改进建议、提交 PR 或分享你的改装版本！

Improvements, PRs, and modified versions are welcome!

### 如何贡献 | How to Contribute

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

## 📄 许可证 | License

本项目采用 [MIT 许可证](./LICENSE)

This project is licensed under the [MIT License](./LICENSE).

---

## 📞 联系方式 | Contact

- **GitHub**: [@Clr168](https://github.com/Clr168)
- **B 站视频**: [演示视频](https://www.bilibili.com/video/BV1EB4y197ZR)
- **闲鱼**: 老 diy 玩家了（已售出整机）

---

## 🙏 致谢 | Acknowledgments

- 感谢 Ultimaker 的 UM2 设计灵感
- 感谢开源 3D 打印社区的支持

---

<div align="center">

**如果这个项目对你有帮助，请给个 ⭐ Star！**

*If this project helps you, please give it a ⭐ Star!*

</div>
