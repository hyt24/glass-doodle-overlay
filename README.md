# Glass Doodle Overlay

A Codex image-editing skill for the “it looks like…” window-doodle effect: preserve a real photograph, then use a handful of thick white marker strokes on the foreground glass to make one subject read as a cute imagined character or object.

## What it creates

The source photograph remains recognisable: its subject, composition, perspective, and lighting stay intact. The edit adds a deliberately simple white drawing aligned to the subject, as though someone standing indoors has casually sketched on the window pane while looking outside.

The effect always protects the depth order:

`foreground glass doodle → real subject outdoors → original background`

By default, generation uses a 4:5 canvas. It avoids replacing the subject, fogging the window, intricate illustration, thin lines, captions, UI elements, and watermarks.

## Install

Clone the repository into a Codex skill directory:

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/glass-doodle-overlay.git \
  ~/.codex/skills/glass-doodle-overlay
```

Or copy this folder to a project-local skill directory such as `.agents/skills/glass-doodle-overlay`.

Restart or refresh Codex if the skill does not appear immediately.

## Use

Attach a photo and invoke the skill, specifying the real subject and the imagined form:

```text
使用 $glass-doodle-overlay：把窗外那辆白色小车想象成一只小狗，保持原图场景不变。
```

```text
Use $glass-doodle-overlay: make the cloud shaped like a whale, with only a few thick white doodle lines on the foreground glass.
```

## Included files

- `SKILL.md` — workflow, editing rules, and quality checks.
- `references/style-guide.md` — scene-preservation and doodle-art-direction rules.
- `references/prompt-template.md` — a reusable generation prompt template.
- `agents/openai.yaml` — Codex UI metadata.

## License

MIT. See [LICENSE](LICENSE).
