# xiaolab-group-meeting-skill

面向使用者的 xiaolab 组会 HTML deck skill。

它的目标很简单：

- 让 AI 帮你做一份 **可直接打开的 HTML 组会 deck**
- 保留 xiaolab / 湖大 / 国家超级计算长沙中心品牌层
- 适合论文、系统、项目进展类组会汇报

可直接交给 `Claude Code`、`Codex`、`Hermes`、`OpenClaw` 这类 agent 使用。

## 仓库内容

- `skill/SKILL.md`：发布版模板 skill
- `template/core/index.html`：极少默认页
- `template/components/index.html`：可拼装组件页
- `template/assets/`：品牌资源与样式
- `references/`：补充设计说明

## 模板特点

- 保留 xiaolab / 湖大 / 国家超级计算长沙中心品牌层
- 16:9 画板，全屏等比缩放
- 干净背景，不允许模板说明文字浮在成品页
- 支持 `← / →`、滚轮、触控横滑、`F` 全屏、`ESC` 总览
- 默认模板只保留封面 / 主内容 / 下一步三页骨架
- 组件页用于扩展双列图文、对照、流程、媒体区等布局

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

## 交付形式

- 一个可直接打开的 HTML 页面
- 默认查看入口：`template/core/index.html`
- 组件查看入口：`template/components/index.html`
- 如有配图，可附同级 `images/` 目录

## 参考说明

- `references/component-patterns.md`：组件族、扩展方向、清洁检查
- `references/template-iteration-lessons-2026-05-06.md`：模板清稿与页面洁净边界

## 使用方式

安装后，直接把这个 skill 交给 `Claude Code`、`Codex`、`Hermes` 或 `OpenClaw`，再附上你的组会主题和材料即可。

## 开源说明

仓库已去掉本地运行环境依赖；如需按你自己的实验室模板继续改，请替换 `template/assets/` 中的品牌资源，并按 `skill/SKILL.md` 调整规则。
