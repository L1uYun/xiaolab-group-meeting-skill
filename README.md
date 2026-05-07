# xiaolab-group-meeting-skill

面向使用者的 xiaolab 组会 HTML deck skill。

它的目标很简单：

- 让 AI 帮你做一份 **可直接打开的 HTML 组会 deck**
- 保留 xiaolab / 湖南大学 / 国家超级计算长沙中心品牌层
- 适合论文、系统、项目进展类组会汇报

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

## 交付形式

- 一个可直接打开的 HTML 页面
- 如有配图，可附同级 `images/` 目录

## 使用方式

安装后，让 AI 读取这个 skill，并按你的组会主题直接生成 deck 即可。
