# Release Notes

## v1.0.0 - 初始发布 (2026-01-15)

### 🎉 首次发布

这是 Markdown Visualizer 插件的第一个正式版本，为 Obsidian 带来强大的可视化能力。

### ✨ 核心功能

#### 1. Canvas 渲染器
- 支持 JSON Canvas 格式
- 节点类型：text, file, link, group
- 6 种颜色预设
- **新特性**：多行文本自动换行和溢出处理

#### 2. Graphviz 渲染器
- 支持 DOT 语言
- 6 种布局引擎（dot, neato, fdp, sfdp, circo, twopi）
- 响应式 SVG 输出
- **新特性**：完善的错误处理机制

#### 3. Infographic 渲染器
- **22+ 种专业模板**
- 完整的 DSL 解析器
- 6 种主题配色方案

**模板列表**：
- 网格布局 (list-grid-*)
- 横向列表 (list-row-*)
- 纵向列表 (list-column-*)
- 时间线 (sequence-timeline-*)
- 步骤 (sequence-steps-*)
- 对比 (compare-*)
- **🆕 漏斗图 (funnel-simple)** - 转化流程分析
- **🆕 进度指标 (progress-bar)** - 项目进度追踪
- **🆕 路线图 (roadmap-vertical)** - 时间线规划
- **🆕 价格表 (pricing-table)** - 定价方案展示

#### 4. Vega 渲染器
- 支持 Vega 和 Vega-Lite
- 自动主题适配
- 可配置交互按钮

### 🎨 设计特性

- **主题集成**：完全适配 Obsidian 深色/浅色主题
- **CSS 动画**：
  - Shimmer 闪光效果（进度条）
  - Pulse 脉冲动画（路线图）
  - 平滑的悬停效果
- **响应式布局**：自动适应不同屏幕尺寸
- **自定义配色**：5 种预设颜色主题

### 📦 安装方法

#### 方式一：手动安装

1. 下载 release 文件
2. 解压到 `.obsidian/plugins/markdown-visualizer/`
3. 在 Obsidian 设置中启用插件
4. 重新加载 Obsidian

#### 方式二：从源码构建

```bash
git clone https://github.com/wangjia15/obsidian-markdown-visualizer.git
cd obsidian-markdown-visualizer
cp -r .obsidian/plugins/markdown-visualizer ~/.obsidian/plugins/
```

### 📖 快速开始

#### Canvas 示例
````markdown
```canvas
{
  "nodes": [
    {"id": "1", "type": "text", "text": "开始", "x": 0, "y": 0, "width": 120, "height": 60}
  ]
}
```
````

#### Infographic 漏斗图示例
````markdown
```infographic
infographic funnel-simple
data
  title 销售转化漏斗
  items
    - label 访问网站
      value 10000
    - label 付费用户
      value 1000
```
````

### 📊 性能指标

- 插件大小: ~3.1 MB
- 支持的渲染器: 4 个
- 支持的代码块类型: 7 种
- 模板数量: 22+ 种
- 配置选项: 10+ 项

### 🐛 已知问题

目前没有已知的严重问题。如发现 bug，请在 [Issues](https://github.com/wangjia15/obsidian-markdown-visualizer/issues) 中报告。

### 🙏 致谢

感谢以下开源项目：
- [Obsidian](https://obsidian.md/)
- [d3-graphviz](https://github.com/magjac/d3-graphviz)
- [Vega](https://vega.github.io/)
- [Vega-Lite](https://vega.github.io/vega-lite/)

### 📝 完整文档

详见 [README.md](README.md)

---

**下载链接**: [v1.0.0 Release](https://github.com/wangjia15/obsidian-markdown-visualizer/releases/tag/v1.0.0)
