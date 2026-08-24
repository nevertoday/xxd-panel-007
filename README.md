<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 007 项目横幅" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 007

### 把照片拆成边看边读、亲切清爽的手写生活观察图谱

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#四种输出共享同一种观察图谱逻辑)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#边界与信任)

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> 实物小图 · 局部／剖面／重复 · 错位留白 · 细黑手写 · 扫描纸感

XXD Panel 007 是一个面向 Codex 与兼容 Agent 的图像生成 Skill。它把同一张照片拆解为若干实物状小图、局部特写、剖面、重复小件和细节片段，松散分布在洁白纸面的中上部与中段。

每个片段保留源图的材料、颜色、圆钝轮廓、轻微透视和手绘痕迹；细黑手写短词、拟声词与注释在图形左右穿插，形成边看边读的亲密节奏。它像绘本信息页与手账实物笔记之间的一页，但不变成图标表或贴纸合集。

## 为什么需要 007

普通“手账风”很容易退化成整齐图标、标准贴纸、统一标签和无关小物堆砌，源照片只是一个可替换主题名。

007 的顺序完全相反：

```text
锁定源图事实 → 选择有信息价值的整体／特写／剖面／重复／细节 → 保留实物材料感 → 在白纸中松散错位 → 用细黑手写串联 → 以扫描柔化和颜料吸收完成
```

如果换成一张无关照片，片段选择、材料线索、手写观察和阅读顺序仍然成立，这张图就不属于 007。

## 007 的视觉契约

- **同源观察片段：** 整体、特写、剖面、重复小件或细节都必须来自同一主体，不固定格数。
- **实物笔记感：** 小尺幅、圆钝轮廓、轻微透视和手绘上色保留材料与识别特征。
- **有证据的细节：** 颗粒、焦边、碎屑、纤维、接缝、反光、纹理或剖面只在源图支持时出现。
- **松散阅读：** 小图主要分布在中上部与中段，以错位留白形成近似横向或符合目标文字方向的节奏。
- **拒绝严整网格：** 不做表格、卡片墙、栏目、居中标本矩阵或统一尺寸图标。
- **文字是骨架：** 细黑手写短词、短句、拟声词和注释左右穿插，字距松弛、基线轻跳。
- **白纸与暖色：** 白纸占最大面积，黑字承担信息，温暖清洁主体色与少量深色或高饱和色承担焦点。
- **扫描手感：** 保留轻微柔化、自然压缩、边缘不齐和颜料吸收，不加厚重阴影、边框或强现代排版。

## 样张 · 来自 X

> [小小东（@xiaoxiaodong01）](https://x.com/xiaoxiaodong01/status/2090005645353468277) · 2026-08-19<br>
> GPT2 x 手账 x 手绘 x 插画 x 拆解 x 美学提示词 x VOL.007

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-01.jpg" alt="XXD Panel 007 样张 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-02.jpg" alt="XXD Panel 007 样张 2"></a></td>
  </tr>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-03.jpg" alt="XXD Panel 007 样张 3"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-04.jpg" alt="XXD Panel 007 样张 4"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277">查看原推文与完整提示词 →</a></p>

这些样张用于展示 007 的美学动机，不会把样张中的主体、构图、配色、文案或旧画幅变成生成参考或当前默认值。

## 四种可组合输出模式

可用 `1`、`1+3`、`1、2、4` 或 `全部` 选择一个或多个模式；`全部` 每张源图输出 7 个独立 PNG。模式确定后，Skill 会在生图前继续询问整张最终成品的画幅：`3:4` 原提示词画幅、明确跟随原图、常用比例，或自定义比例／准确像素。不会再静默套用源图尺寸。

| 模式 | 画幅逻辑 | 成品 |
| --- | --- | --- |
| `top-bottom` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在上，007 设计在下，约 50/50 |
| `left-right` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在左，007 设计在右，约 50/50 |
| `design-only` | 用户确认的整张成品画幅 | 007 设计铺满画布，不显示原照片 |
| `wallpaper-pack` | 逐设备确认 | 手机、iPad、电脑、儿童手表四张独立 PNG |

双联默认把原图作为高保真垫图／编辑参考，用一套完整提示词直接生成一张整体成品，让摄影、设计、色彩、光线、文字与含义自然呼应。只有完整画布针对性重试仍失败、用户要求原片逐像素不变、当前通道无法实现目标画幅，或需要无创像素校准时，才启用确定性拼合兜底。

壁纸可选连贯或独立。连贯套装先批准一张 iPad 定调图，另外三张分别参考原图＋同一定调图重新构图；独立套装的四张都只参考原图。两者都不会裁切其他设备成品或串联衍生图。

## 文字必须让观众边看边读

正式生图前，先选择自动文案、自定义文案或无文字。有文字时还要指定目标语言或地区。

自动文案从可见材料、动作、功能、关系、可信感官暗示或已知上下文提炼少量短词、短句、拟声词和注释。感官与记忆性文字必须有图像证据或用户信息支持。

默认只有一个标题；只有确有信息价值时才增加零至两条短注释，不会为了显得高级而编造编号、年份、坐标或档案标签。文案仍需通过换图测试。

用户提供最终成稿时逐字保留。用户提供的是方向或可编辑草稿时，才会在保留受众、目的、必备词、语气和潜台词的前提下专业深化。

语言遵循目标受众，而不是用户下指令时使用的语言：

```text
目标市场或受众 > 指定成品语言 > 用户方向语言；都不明确时生图前询问
```

日本版使用自然日语，韩国受众使用自然韩语与正确空格，英国版使用英式英语，阿拉伯语版默认使用自然的现代标准阿拉伯语和真正的从右到左排版。字体会在当地文字系统中保持安静、低密度的书封感，而不是把拉丁规则生硬套过去。

## 完整画布优先与位图边界

图像模型负责整张成品的审美重构，双联也默认一次直出完整画布。`scripts/compose_panel.py` 只保留为条件明确的兜底、无创尺寸校准和只读审计工具，不再预先规划每次任务，也不评价审美是否成功。

全部交付为 PNG 位图。每次调用都在 `~/Desktop/xxd/` 下创建新任务；已配置图像通道只返回脱敏状态，不公开供应商、端点、凭据、请求头、提示词、响应或账户信息。SVG、HTML、Canvas、图表和程序绘图不能替代最终作品。

## 生图模型优先级

GPT Image 2 是默认首选，并继续执行本项目现有的高保真垫图、生成前确认整张画幅、双联一次生成完整画布、脚本仅作条件式兜底等逻辑。

当当前工具或已配置兼容通道确实可用，并能满足原图保真、整张成品比例、目标语言文字和连贯壁纸多图参考等要求时，也支持 Seedance 5.0 Pro、Nano Banana Pro（Gemini Image Pro）、Nano Banana 2（Gemini Image Flash）或其他兼容位图模型。备用模型只替换生成通道，不得改变模式、画幅、文案、语言、壁纸关系和完整画布优先策略。

如果没有合适的生图通道，Skill 会请用户启用生图工具或提供 API Key。用户主动提供的凭据可以用于当前任务，但不得在回复或日志中回显、展示或泄露；未经用户明确要求，不会长期保存凭据或修改供应商、账户、计费及全局路由配置。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-007.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-007" ~/.codex/skills/xxd-panel-007
```

Claude Code 用户可以把同一目录链接到 `~/.claude/skills/xxd-panel-007`。安装后重新启动 Agent 会话。

```text
$xxd-panel-007
把这张照片做成左右双联，文案由你根据照片内涵创作，使用自然韩语。
```

只上传照片也可以调用。Skill 会先用分行编号菜单询问一个或多个模式，再询问文字设置；选择壁纸时还会确认连贯或独立以及设备尺寸。

完整规范：

- [Skill 工作流](SKILL.md)
- [中文完整提示词](references/xxd-panel-007-prompt.zh-CN.md)
- [英文完整提示词](references/xxd-panel-007-prompt.en.md)
- [原始风格提示词](references/007-source.md)

## 边界与信任

- 每张照片只在自己的任务中使用，不借用其他输入、旧成品或样张里的主体、颜色、文案和构图。
- 每次调用都创建新的任务子文件夹；相同原图和参数也要重新生成，旧成品不能冒充当前任务。
- 最终交付为 PNG 位图，不是 SVG、HTML、Canvas 或程序绘图替代品。
- 已配置位图桥接只返回脱敏状态，不显示供应商、端点、请求头、凭据、提示词或服务器响应正文。
- 每个所选普通模式各返回一张；若选择 `wallpaper-pack`，再返回四张独立壁纸。选择 `全部` 时每张原图共返回 7 个 PNG，分处四个同级模式文件夹，绝不生成拼贴总览。

本地拼版需要 Python 3 和 Pillow。安全位图桥接使用 Python 3.11+ 的 `tomllib`。图像生成仍需要主机 Agent 的内置位图能力或已经配置好的兼容位图路径。

## 项目结构

```text
xxd-panel-007/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/（未来本地样张占位）
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-007-prompt.zh-CN.md
    ├── xxd-panel-007-prompt.en.md
    └── 007-source.md
```

## 关于 XXD

XXD 是小小东的品牌名称缩写。项目由 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01) 创建并维护。

## 服务与会员

### 深度咨询 · 299 元/小时

Skills 使用的一对一深度咨询按 299 元/小时收费。请通过下方微信二维码联系小小东预约。

### 小小东 Skills 用户交流群 · 入群 99 元

一次支付 99 元加入用户交流群，用于交流工作流、作品与互助；不包含按小时的一对一深度咨询。扫码后请备注“Skills 用户交流群”。

### 知识星球＋成员提示词库 · 699 元/年

[知识星球](https://wx.zsxq.com/group/15554814142882)与[小小东成员提示词库](https://vip.xiaoxiaodong.ai/)是同一份会员权益：**一次年费同时开通两边，无需重复付费。**

1. 在[知识星球](https://wx.zsxq.com/group/15554814142882)开通后，微信联系小小东领取成员提示词库兑换码。
2. 在[成员提示词库](https://vip.xiaoxiaodong.ai/)自助开通后，微信联系小小东邀请进入知识星球。

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="小小东付费服务微信二维码" width="320"></a>
</p>

<div align="center">

**不是把物件排成一列，而是把观看它的过程留在纸上。**

</div>

---

<div align="center">
  <h2>☕ 为开源项目赞助算力</h2>
  <p>如果这个项目为你节省了时间，可以通过微信或支付宝赞助后续测试与生成算力。</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png" alt="小小东微信算力赞助二维码" width="180"></a><br>
        <strong>微信算力赞助</strong>
      </td>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png" alt="小小东支付宝算力赞助二维码" width="180"></a><br>
        <strong>支付宝算力赞助</strong>
      </td>
    </tr>
  </table>
  <p><sub>赞助完全自愿，不会改变这个开源项目的使用权限。</sub></p>
</div>
