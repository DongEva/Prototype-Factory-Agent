# Prototype Factory Agent

**交互展项原型生成 Agent** — 将展项描述转化为可运行的单文件 HTML 低保真原型。

An AI agent that converts museum/exhibition descriptions into runnable single-file HTML lo-fi prototypes.

---

## 🔥 Prototype Factory Agent: The Ultimate Multi-Screen Interaction Demo Tool


## 🚀 Why This Project Exists

Tired of explaining complex multi-screen, multi-device interactive designs with boring PPTs?
Sick of spending hours manually building low-fidelity prototypes that still don't make sense to clients?
I built this Prototype Factory Agent to fix this exact pain point for every interaction designer, multimedia creator, and exhibition developer.
## ✨ Key Features That Make It a Game-Changer

• 🖥️ One-Click Multi-Device Linkage: Auto-sync logic across screens, consoles, buttons, and physical installations

• 🎯 Instant Interactive Low-Fi Demos: Generate shareable, clickable prototypes in minutes, no manual debugging

• 📊 Presentation-First Design: Cast directly to screens for client meetings, logic flows clear at a glance

• 💰 Massive Time & Cost Savings: Validate logic with low-fi first, avoid costly high-fidelity rework

• 🌐 HTML-Powered Presentations: Your next presentation doesn't have to be a PPT—interactive demos > static slides
## 🎯 Who Is This For?

• 🎨 Interaction & Multimedia Designers

• 🏛️ Exhibition & Installation Developers

• 📱 UI/UX Designers working on cross-device experiences

• 🧑‍💻 Product Managers needing to demo complex workflows

• 🎓 Educators teaching multi-screen interaction logic
## 💡 Core Philosophy

Your next presentation doesn't have to be a PPT.
Interactive, HTML-based demos are the future of presenting complex interactive systems—more intuitive, more convincing, and way more professional than static slides.
## 📦 Use Cases

• Multi-screen exhibition & smart space solution demos

• Physical installation interaction logic verification

• Cross-device product interaction prototype generation

• Client proposal & team alignment presentations

• Teaching & training for interactive design workflows
## 🤝 Contribute & Star

If this tool solves your pain point, give it a ⭐ Star!
Contributions, feature requests, and feedback are all welcome to make this tool even better for the design community.
## 🏷️ Tags
Agent Prototype Tool Interaction Design Multi-Screen Multimedia Low-Fi Prototype HTML Presentation Design Efficiency UI/UX Open Source Exhibition Design
中文版（GitHub开源爆款优化版）

🔥 原型图工厂 Agent：多屏交互演示神器，设计师效率天花板

🚀 为什么做这个工具？

做多媒体交互、多屏联动、装置交互的设计师们，谁没被这些痛点折磨过？
用PPT讲复杂联动逻辑，客户听不懂、团队难对齐，越讲越乱；
手动做低保真原型，挨个调屏、连逻辑、改流程，熬夜赶工还不直观；
直接上高保真，方案一改全白费，时间和资源全浪费在无效试错上。

于是我做了这个原型图工厂Agent，专门解决多设备联动演示的世纪难题！
## ✨ 核心亮点，直接封神

• 🖥️ 多设备联动一键生成：自动串联多屏、中控、按钮、实体装置的交互逻辑，不用手动逐个调试

• 🎯 可交互低保真Demo秒出：几分钟生成可点击、可演示的原型，投屏即懂，汇报说服力拉满

• 💰 从源头省时间省资源：先用低保真跑通全流程，再做高保真/交付开发，彻底避免返工

• 🌐 HTML交互汇报新范式：你的下一个汇报PPT，何必是PPT！交互式演示直接吊打静态PPT
## 🎯 谁用谁香？

• 🎨 多媒体/交互/展厅设计师

• 🏛️ 装置艺术、智慧空间开发者

• 📱 跨端体验UI/UX设计师

• 🧑‍💻 需要演示复杂流程的产品经理

• 🎓 交互设计教学与培训从业者
## 💡 核心理念

你的下一个汇报PPT，何必是PPT。
更直观、更真实的HTML交互汇报，正在彻底替代传统PPT，成为复杂交互设计方案演示的新标准。
## 📦 适用场景

• 多屏展厅、智慧空间方案汇报

• 实体装置交互逻辑验证与演示

• 跨端产品交互原型快速生成

• 客户提案、团队需求对齐

• 交互设计教学与培训演示
## 🤝 开源共建

如果这个工具解决了你的痛点，欢迎给项目点个⭐ Star！
欢迎提交Issue、PR，一起把它打造成设计师圈的效率神器！
🏷️ 标签
Agent 原型工具 交互设计 多屏联动 多媒体交互 低保真原型 HTML汇报 设计提效 UI/UX 开源 展厅设计

## 什么是它 / What it does

你只需要描述一个展项（名称、设备类型、交互方式、内容类型、自动复位时间），Agent 会通过对话补全信息，然后生成一个可直接在浏览器打开的 HTML 原型文件。

You describe an exhibit (name, device type, interaction method, content type, auto-reset timing), and the agent fills in missing details through conversation, then outputs a ready-to-run HTML prototype.

**生成的原型包含 / Each prototype includes:**
- 1920×1080 固定布局，黑/白/灰低保真风格
- 左侧硬件流程图 + 右侧设备模拟区
- 四状态机：待机 → 触发 → 展示 → 自动复位
- 多媒体标注面板（音效 / 灯光 / 动画）
- 所有文字双击可直接编辑

---

## 文件说明 / File Structure

```
Prototype-Factory-Agent/
├── agent-prompt.txt          # Agent 系统提示词（粘贴到任何支持 system prompt 的工具）
├── prototype-agent.html      # 可视化演示界面（直接浏览器打开）
├── template/
│   └── interactive-exhibit-lofi.html   # 低保真原型框架模板
└── examples/
    └── (可放置你生成的示例原型)
```

---

## 快速开始 / Quick Start

### 方式一：使用 Claude Code（推荐）

1. 安装 [Claude Code](https://claude.ai/code)
2. 在项目目录打开终端，启动 Claude Code
3. 将 `agent-prompt.txt` 内容作为 system prompt，或直接告诉 Claude：
   > "请扮演交互原型 Agent，按照 agent-prompt.txt 的规则工作"
4. 描述你的展项，Agent 会引导你完成信息收集并生成 HTML

### 方式二：其他 AI 工具

将 `agent-prompt.txt` 的内容粘贴为 system prompt，在任何支持自定义 system prompt 的 AI 工具中使用（ChatGPT、Cursor、API 调用等）。

### 查看演示界面

直接用浏览器打开 `prototype-agent.html` 可以看到 Agent 对话界面的视觉原型。

---

## 工作流程 / Workflow

```
用户描述展项需求
      ↓
Agent 提取结构化信息
      ↓
信息完整后生成单文件 HTML
      ↓
浏览器直接打开预览 → 双击文字编辑 → 截图/演示
```

---

## 适用场景 / Use Cases

- 博物馆 / 科技馆互动展项设计方案演示
- 向客户说明展项交互逻辑与硬件布局
- 内部评审用低保真原型
- 快速验证展项创意

---

## License

MIT
