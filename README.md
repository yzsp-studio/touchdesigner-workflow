<div align="center">

# 🎬 touchdesigner-workflow

## 6 步把 TD 工程从零搭到能交付，节点错误一个不漏
## 6 steps from blank TouchDesigner project to shippable, node errors caught

📮 **商务合作 / Business：wow.vip@foxmail.com**
🎬 **抖音 / Douyin：[v.douyin.com/07EjIDGVErY](https://v.douyin.com/07EjIDGVErY/)**

</div>

---

## 🇨🇳 中文

这是 TouchDesigner 实时视觉与交互工程的作业流程技能，覆盖从环境准备、节点选型、分阶段制作到导出交付的全链路。它先用脚本发现在 Windows/macOS 上已安装的实例并复用唯一运行中的一个，遇到多实例或监听冲突时直接停止写入，而不是覆盖别人的工程。选型阶段给出一张「效果目标 → 节点家族」矩阵，把颜色纹理、曲线粒子、参数动画、脚本数据、GLSL 自定义效果和 UI 控件分别对应到 TOP、SOP/POP、CHOP、DAT、GLSL TOP 与 COMP 的正确链路。制作时每改一段就回读节点、连线、参数实际值和父网络错误，导出前核对编码器与像素格式，硬件编码不可用时退到 ProRes、MJPEG 或 PNG 序列并说明是否要外部转码。只有当用户明确选择 TouchDesigner 时才触发，交付可编辑工程加媒体与依赖清单。

### ✨ 能做什么

- 效果目标 → 节点家族矩阵：颜色、粒子、参数动画、脚本、GLSL、UI 各走哪条链路一表定路线
- Windows/macOS 一键发现并启动 TD，复用唯一实例，多实例或监听冲突时停止写入
- 每改一段就回读节点、连线、参数实际值和父网络错误，不凭旧版本记忆写参数
- 导出前核对编码与像素格式，硬件 H.264/H.265 不可用自动换 ProRes、MJPEG、PNG 序列
- 故障按输入 → 通道 → 表达式 → 连线 → 合成 → 输出 → 父网络逐层定位，6 类现象各有优先检查项
- 交付可编辑 .toe 与按需 .tox 加媒体清单，Mac 通过不算 Windows 通过，逐项分别报告

### 📦 包含的技能

- `touchdesigner-workflow` —— 见 [`touchdesigner-workflow/SKILL.md`](touchdesigner-workflow/SKILL.md)

### 🚀 安装

```bash
git clone https://github.com/yzsp-studio/touchdesigner-workflow.git
cp -r touchdesigner-workflow/* "$DSH_HOME/skills/"
```

> 技能是**纯文本说明**（`SKILL.md` + `references/`），零依赖、零 API key，用你当前 agent 的会话额度。

---

## 🇬🇧 English

This skill is the working procedure for TouchDesigner realtime visual and interactive builds, covering environment prep, node selection, staged production, and export. It uses bundled scripts to find an installed app on Windows or macOS and reuse the single running instance, stopping writes outright when multiple instances or listener conflicts appear instead of clobbering someone else's project. For selection it ships an effect-goal-to-node-family matrix that maps colors and textures, curves and particles, parameter animation, script data, custom GLSL effects, and UI controls onto the right TOP, SOP/POP, CHOP, DAT, GLSL TOP, and COMP chains. During production it re-reads nodes, wires, parameter values, and parent-network errors after every stage, and before export it checks encoder and pixel format, falling back to ProRes, MJPEG, or PNG sequences when hardware encoding is unavailable. It triggers only when the user actually chooses TouchDesigner, and it delivers an editable project plus a media and dependency list.

### ✨ What it does

- Effect-goal-to-node-family matrix: one table routes colors, particles, parameter animation, scripts, GLSL, and UI
- Finds and launches TouchDesigner on Windows or macOS, reuses the single instance, and stops writing on multi-instance or listener conflicts
- Re-reads nodes, wires, actual parameter values, and parent-network errors after every stage instead of writing from memory
- Checks encoder and pixel format before export; falls back to ProRes, MJPEG, or PNG sequences when hardware H.264/H.265 is unavailable
- Triage walks input, channels, expressions, wiring, compositing, output, then parent-network errors, with priority checks per symptom
- Delivers an editable .toe plus .tox when reuse matters, with a media list; a Mac pass never counts as a Windows pass

### 📦 Skills included

- `touchdesigner-workflow` — [`touchdesigner-workflow/SKILL.md`](touchdesigner-workflow/SKILL.md)

### 🚀 Install

```bash
git clone https://github.com/yzsp-studio/touchdesigner-workflow.git
cp -r touchdesigner-workflow/* "$DSH_HOME/skills/"
```

> Skills are **plain-text instructions** (`SKILL.md` + `references/`). Zero dependencies, no API keys — they run on your agent's existing session quota.

---

## 📮 联系 / Contact

| | |
|---|---|
| 🎬 **抖音 / Douyin** | [https://v.douyin.com/07EjIDGVErY/](https://v.douyin.com/07EjIDGVErY/) |
| 📮 **商务合作 / Business** | **wow.vip@foxmail.com** |
| 🐙 **GitHub** | [https://github.com/yzsp-ai](https://github.com/yzsp-ai) |
| 💖 **打赏 / Support** | [afdian.com/a/yzsp-ai](https://afdian.com/a/yzsp-ai) |

## 📄 License

[MIT](LICENSE) · © 2026 [yzsp-ai](https://github.com/yzsp-ai)
