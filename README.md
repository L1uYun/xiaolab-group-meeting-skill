# xiaolab-group-meeting-skill

Xiaolab 组会 HTML 模板与配套 skill。

## 含什么

- `skill/SKILL.md`：模板工作流与规则
- `template/index.html`：单文件 HTML deck 模板
- `template/assets/`：品牌资源与样式
- `references/`：方法与拆解笔记

## 模板特点

- 保留 xiaolab / 湖南大学 / 国家超级计算长沙中心品牌层
- 干净背景；不允许提示语、残影、说明字浮在成品页
- 16:9 画板，全屏等比缩放
- 双层结构：`core/` 默认页 + `components/` 组件页
- 封面使用模板变量：
  - `{{第几次组会}}`
  - `{{姓名}}`
  - `{{起始日期}}`
  - `{{结束日期}}`

## 页面结构

### core

1. 封面
2. 主内容页
3. 下一步页

### components

- 双列图文
- 双图对照
- 三栏带
- 四格媒体区
- 上下分栏
- 流程带
- 对照区

## 使用

直接打开 `template/index.html` 即可预览。

交互：

- `← / →` 翻页
- 滚轮 / 触控横滑
- `F` 全屏
- `ESC` 打开详情卡总览

## 开源说明

仓库已去掉本地运行环境依赖；如需按你自己的实验室模板继续改，请替换 `template/assets/` 中的品牌资源，并按 `skill/SKILL.md` 调整规则。
