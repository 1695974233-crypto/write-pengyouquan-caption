# 朋友圈文案生成 Skill

一个面向 Codex 的中文朋友圈文案生成 Skill。它能够理解文字、图片或图文混合素材背后的场景、情绪和分享意图，生成自然、贴切、可以直接发布的朋友圈文案。

## 能做什么

- 根据文字、单张图片、多张图片或图文混合素材生成文案
- 判断旅行、日常、美食、聚会、节日、工作感悟等场景
- 默认提供诗意版、简短版和氛围版三种候选
- 支持诗句、名人名言、自然口语、含蓄表达、小红书感和抖音感
- 核验诗词和名言，避免错字、错作者和伪名言
- 避免模板腔、过度矫情、无依据推断和文案同质化

## 示例

输入：

> 今天去西湖散步，帮我生成朋友圈文案。

输出示例：

> **诗意版：** 最爱湖东行不足，绿杨阴里白沙堤。
>
> **简短版：** 风从西湖来，今天也慢慢走。
>
> **氛围版：** 没有赶路，只是在湖边把今天过得慢一点。

也可以上传图片后输入：

> 根据这张照片写一句克制、不矫情的朋友圈文案。

## 安装

将仓库克隆到 Codex 的 Skills 目录：

```bash
git clone https://github.com/1695974233-crypto/write-pengyouquan-caption.git ~/.codex/skills/write-pengyouquan-caption
```

重新打开 Codex 任务后，即可在可用 Skills 中看到“朋友圈文案生成”。

## 使用

显式调用：

```text
使用 $write-pengyouquan-caption，根据这段文字或图片生成三条朋友圈文案。
```

当请求明显属于朋友圈配文、旅行打卡、日常记录或已有文案润色时，Codex 也可以自动调用该 Skill。

## 项目结构

```text
write-pengyouquan-caption/
├── SKILL.md                  # Skill 核心工作流
├── agents/openai.yaml        # Codex 界面元数据
├── references/style-guide.md # 风格规范和质量检查
├── README.md                 # GitHub 项目说明
└── LICENSE                   # CC0 1.0 Universal
```

## 许可证

本项目采用 [CC0 1.0 Universal](LICENSE)。你可以自由复制、修改、商用和再分发，基本无须申请授权或保留署名。

`SKILL.md` 是 Codex 执行本 Skill 时读取的核心文件；`README.md` 仅用于 GitHub 项目展示和安装说明。
