<p align="center">
  <img src="assets/huixi_logo_cropped.png" alt="辉羲智能" height="72" />
</p>

<h1 align="center">
  <img src="assets/rhinovla_logo.png" alt="RhinoVLA logo" height="56" style="vertical-align:middle;" />
  RhinoVLA
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/License-Apache--2.0-green" alt="License" />
  <a href="https://arxiv.org/abs/2606.07383"><img src="https://img.shields.io/badge/Paper-arXiv%202606.07383-red" alt="Paper" /></a>
</p>

<p align="center">
  <b>中文</b> |
  <a href="./README_EN.md">English</a> |
  <a href="https://arxiv.org/abs/2606.07383">Paper</a>
</p>

<p align="center">
  <b>面向机器人端侧实时控制的跨本体 Vision-Language-Action 模型</b>
</p>

RhinoVLA 是辉羲智能自研的跨本体 VLA 系统，面向机器人本体端实时控制设计。技术报告展示了辉羲自研 VLA、辉羲 R1 芯片，以及智元、银河通用机器人组成的模型-芯片-机器人部署链路。

RhinoVLA 在辉羲 R1 芯片上实现了 **11.69Hz** 端到端推理频率，跨过机器人实时闭环控制常用的 10Hz 门槛。同时，RhinoVLA 通过统一状态-动作接口和实例适配机制，支持同一策略迁移到不同机器人平台。

## 主要特性

- **端侧实时部署**：围绕机器人本体端运行设计，在 R1 芯片上实现实时 VLA 推理。
- **算法-系统联合优化**：采用 Qwen3-VL Backbone + Action Expert 结构，并结合芯片、算子和运行时优化降低端侧开销。
- **跨本体适配**：通过 View Registry、72D 状态-动作接口和 Instance LoRA 处理视觉输入、动作接口和机器人实例差异。

<p align="center">
  <img src="assets/rhinovla_architecture.png" alt="RhinoVLA architecture" width="95%" />
</p>

## 🎬 演示 Demo

### Galbot G1：指令跟随

RhinoVLA 运行在银河 G1 与辉羲 R1 芯片上，连续执行三次自然语言指令。

<div align="center">
  <video src="https://github.com/user-attachments/assets/5cc67652-53a8-49a0-a38c-08ae5fc38f68" width="100%" controls></video>
</div>

### AgiBot G2：长程任务

RhinoVLA 运行在智元 G2 与辉羲 R1 芯片上，通过一次长指令完成多步骤任务。

<div align="center">
  <video src="https://github.com/user-attachments/assets/04499b63-fefd-498d-8bd2-fdab28c1c2dd" width="100%" controls></video>
</div>

### AgiBot G1：双臂叠毛巾

RhinoVLA 运行在智元 G1 与辉羲 R1 芯片上，完成双臂柔性物体操作。

<div align="center">
  <video src="https://github.com/user-attachments/assets/de229167-6e2d-4e5c-849c-334d9d6800ab" width="100%" controls></video>
</div>

## 📦 Release Plan

- [ ] 模型训练代码
- [ ] 模型参数
- [ ] 训练与评测数据集

## 📄 Citation

如果 RhinoVLA 对你的研究有帮助，请引用我们的技术报告：

```bibtex
@misc{intelligence2026rhinovlatechnicalreport,
      title={RhinoVLA Technical Report}, 
      author={Huixi Intelligence and Chen Zhang and Chenyang Zhou and Guanglei Ding and Guanghui He and Haibin Gao and Jiajia Chen and Jianyong Zhang and Lianyi Yu and Ningyi Xu and Ping Xu and Qingchen Li and Yingjun Hu and Yijia Zhang and Yuxi Liu},
      year={2026},
      eprint={2606.07383},
      archivePrefix={arXiv},
      primaryClass={cs.RO},
      url={https://arxiv.org/abs/2606.07383}, 
}
```

## ⚖️ License

本项目采用 Apache-2.0 License。

## 💬 Contact

微信公众号：

<p align="left">
  <img src="assets/huixi_wechat_qrcode.png" alt="辉羲智能微信公众号二维码" width="360" />
</p>
