# xiaolab-group-meeting-skill

面向使用者的 xiaolab 组会 HTML deck skill。

默认目标很简单：

- 让 AI 帮你做一份 **可直接打开的单文件 HTML 组会 deck**
- 保留 xiaolab / 湖南大学 / 国家超级计算长沙中心品牌层
- 不要求你先理解模板仓库结构

## 最终交付是什么

默认最终交付是：

- 一个 `index.html`
- 如有配图，再配一个同级 `images/` 目录

不是默认交付：

- `core/index.html`
- `components/index.html`
- 多份模板拆页

`template/components/index.html` 只是布局参考页，不是普通用户最终产物。

## 仓库里有什么

- `SKILL.md`：给 Agent 的主工作流
- `template/index.html`：默认单文件模板
- `template/components/index.html`：可选布局参考页
- `template/assets/`：品牌资源与字体
- `references/`：组件说明和质检清单

## 模板特点

- 保留 xiaolab / 湖大 / 国家超级计算长沙中心品牌层
- 16:9 画板，全屏等比缩放
- 干净背景，不允许模板说明文字浮在成品页
- 支持 `← / →`、滚轮、触控横滑、`F` 全屏、`ESC` 总览
- 默认模板只保留封面 / 主内容 / 下一步三页骨架

## 安装

推荐直接把整个仓库克隆到本地 skills 目录，这样模板、资源和 references 都是闭合可用的。

### Codex

```bash
git clone https://github.com/L1uYun/xiaolab-group-meeting-skill.git ~/.codex/skills/xiaolab-group-meeting-skill
```

### Claude Code

```bash
git clone https://github.com/L1uYun/xiaolab-group-meeting-skill.git ~/.claude/skills/xiaolab-group-meeting-skill
```

## 触发方式

这些说法都适合触发：

- “帮我做一份 xiaolab 风格组会 deck”
- “做一个组会 HTML 页面”
- “做一份实验室组会 PPT，但是用网页翻页形式”
- “按 xiaolab 风格整理这次论文/系统汇报”

## 使用方式

1. 让 AI 读取这个 skill
2. 以 `template/index.html` 为起点生成你的成品
3. 如果默认骨架不够，再参考 `template/components/index.html` 补布局
4. 最终仍回到一个单独的 `index.html`

## 预览

直接打开 `template/index.html` 就能看默认模板。  
直接打开 `template/components/index.html` 就能看布局参考页。
