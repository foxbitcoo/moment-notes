# Moment Notes（此刻小记）

一句话描述：
把照片里的“一个时刻”变成有情绪的轻注释，适合朋友圈和社交平台分享。

One-line description:
Turn a photo moment into lightweight emotional notes for social sharing.

`moment-notes` 是一个用于图片情绪注释的 Codex 技能。  
它会把一张照片中的瞬间，转成更有表达力的手绘感注释内容，核心能力包括：

- 场景理解
- 情绪映射
- 横竖屏视角一致的文字排布

`moment-notes` is a Codex skill for emotional photo annotations.
It turns a single image moment into lightweight hand-drawn notes with:

- scene understanding
- emotion mapping
- orientation-aware text layout (landscape vs portrait)

## 通用安装（IDE / Agent） / Universal Install (IDE / Agent)

如果你不是只用 Codex，可以直接用下面这条通用方式：
If you are not using only Codex, use this universal setup:

```bash
git clone https://github.com/foxbitcoo/moment-notes.git
```

然后在你的 IDE / Agent 工具里，把 `moment-notes` 目录作为技能目录或本地能力目录加载。  
Then load the `moment-notes` folder in your IDE/agent as a local skill/capability directory.

常见用法（统一思路）：
Common pattern:
- Cursor: add this repo as a local prompt/skill source
- Claude Code: reference this repo folder as a reusable skill prompt pack
- Codex: install from GitHub URL or copy folder into your skills directory

## 在 Codex 中安装 / Install in Codex

使用下面的 GitHub 地址安装：
Install with this GitHub URL:

```bash
python <path-to-skill-installer>/scripts/install-skill-from-github.py --url https://github.com/foxbitcoo/moment-notes/tree/main
```

如果你的 Codex 环境已经支持 `$skill-installer`，也可以直接让它安装：
If your Codex environment already supports `$skill-installer`, you can ask:

```text
Install this skill from GitHub:
https://github.com/foxbitcoo/moment-notes/tree/main
```

安装后请重启 Codex，让技能生效。  
After install, restart Codex to load the new skill.

## 如何触发 / How to Trigger

你可以用两种方式触发：
You can trigger it in two ways:

1. Explicitly mention skill name:
```text
Use $moment-notes to annotate this photo.
```

2. Natural language request that matches the skill description:
```text
Please add emotional hand-drawn notes to this image with scene understanding.
```

## 能力说明 / What It Does

中文：
- 理解画面里的可见元素和背后场景
- 提炼整张图统一的情绪线
- 让局部注释围绕同一情绪方向
- 文字方向和图片横竖屏保持一致
- 最后输出一句整体情绪总结

English:
- Understands visible objects and hidden scene context
- Builds one unified emotional line for the image
- Keeps all local notes aligned with the same mood
- Matches text direction to image orientation
- Ends with one emotional summary sentence

## 提示词位置 / Prompt Source

核心提示词在：
Core prompt templates are in:

- `references/prompts.md`

## 仓库结构 / Repository Structure

```text
moment-notes/
  SKILL.md
  agents/openai.yaml
  references/prompts.md
  README.md
```

## 备注 / Notes

- 如果你希望别人直接安装，仓库建议设为 `public`。
- 如果仓库是 `private`，别人需要访问权限或 token 才能安装。
- Public repo is required for easy open install by other users.
- If the repo is private, users need access permission or token.
