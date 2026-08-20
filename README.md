# 玻璃涂鸦叠画 / Glass Doodle Overlay

一个 Codex 生图编辑 skill：保留真实照片，并在近处玻璃表面用几笔极粗的白色线条补画，让主体自然呈现“它看起来像……”的可爱联想效果。

A Codex image-editing skill for the “it looks like…” window-doodle effect: preserve a real photograph, then use a handful of thick white marker strokes on the foreground glass to make one subject read as a cute imagined character or object.

## 效果 / What it creates

原图的主体、构图、透视和光线保持不变。画面像摄影者在室内隔着窗户向外看，然后顺手在窗玻璃上补画；线条与窗外真实主体对齐，但不会把主体直接替换成完整动物或奇幻角色。

The source photograph remains recognisable: its subject, composition, perspective, and lighting stay intact. The edit adds a deliberately simple white drawing aligned to the subject, as though someone standing indoors has casually sketched on the window pane while looking outside.

始终维持清晰的空间层次 / The effect always protects the depth order:

`玻璃表面手绘线条 → 窗外真实主体 → 原始环境背景`
`foreground glass doodle → real subject outdoors → original background`

默认画幅为 4:5。主体附近默认会补充 1–5 个与想象形象强相关的极简白色小图标；只有用户明确要求时才不添加。效果避免修改主体、厚重雾气、水汽、复杂插画、细线稿、文字、UI 元素和水印。

By default, generation uses a 4:5 canvas and adds 1–5 tiny white icons strongly related to the imagined form near the subject, unless the user explicitly opts out. It avoids replacing the subject, fogging the window, intricate illustration, thin lines, captions, UI elements, and watermarks.

## 安装 / Install

将仓库克隆至 Codex skills 目录 / Clone the repository into a Codex skill directory:

```bash
git clone https://github.com/hyt24/glass-doodle-overlay.git \
  ~/.codex/skills/glass-doodle-overlay
```

也可以复制到项目本地技能目录，例如 `.agents/skills/glass-doodle-overlay`。

Or copy this folder to a project-local skill directory such as `.agents/skills/glass-doodle-overlay`.

如果没有立即出现，请重启或刷新 Codex。 / Restart or refresh Codex if the skill does not appear immediately.

## 使用 / Use

上传照片后调用 skill，并说明真实主体和要联想的形象。 / Attach a photo and invoke the skill, specifying the real subject and the imagined form:

```text
使用 $glass-doodle-overlay：把窗外那辆白色小车想象成一只小狗，保持原图场景不变。
```

```text
Use $glass-doodle-overlay: make the cloud shaped like a whale, with only a few thick white doodle lines on the foreground glass.
```

## 文件说明 / Included files

- `SKILL.md` — 工作流、编辑规则和质量检查 / workflow, editing rules, and quality checks.
- `references/style-guide.md` — 原图保持与涂鸦视觉规范 / scene-preservation and doodle-art-direction rules.
- `references/prompt-template.md` — 可复用的生图提示词模板 / a reusable generation prompt template.
- `agents/openai.yaml` — Codex 界面元数据 / Codex UI metadata.

## 许可证 / License

MIT. See [LICENSE](LICENSE).
