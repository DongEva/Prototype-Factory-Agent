# Prototype Factory Agent

**交互展项原型生成 Agent** — 将展项描述转化为可运行的单文件 HTML 低保真原型。

An AI agent that converts museum/exhibition descriptions into runnable single-file HTML lo-fi prototypes.

---

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
Agent 提取结构化信息（最多每轮问 3 个问题）
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
