# Cinematic Studio Website Skill

An installable Codex skill that turns a person's own studio, portfolio, or creative-business information into a dark, cinematic React landing page. It preserves the supplied Prisma prompt as a design reference while making the identity, copy, services, calls to action, colors, and media reusable inputs.

## Install

Give the GitHub repository link to Codex and ask:

```text
Install the cinematic-studio-website skill from this GitHub repository:
<REPOSITORY_URL>
The skill is in cinematic-studio-website/.
```

Or use the bundled installer directly:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo OWNER/REPOSITORY \
  --path cinematic-studio-website
```

Restart Codex after installation.

## Use

Invoke the skill and provide whatever information you have:

```text
Use $cinematic-studio-website to build my website.

Brand: Northline Films
Description: A documentary studio focused on climate and human stories.
CTA: Start a project, linking to mailto:hello@example.com
Services: Documentary production, field cinematography, post-production
Colors: Black, warm ivory, muted forest green
Hero media: /path/to/reel.mp4
```

The full optional intake is in [`cinematic-studio-website/references/intake.md`](cinematic-studio-website/references/intake.md). The original supplied prompt is preserved in [`cinematic-studio-website/references/original-prompt.md`](cinematic-studio-website/references/original-prompt.md).

## Repository Layout

```text
cinematic-studio-website-skill/
├── README.md
├── PROJECT_STRUCTURE.md
└── cinematic-studio-website/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── intake.md
        └── original-prompt.md
```

## License

MIT. The reference prompt includes third-party media URLs for design context; recipients should supply media they have permission to use.
