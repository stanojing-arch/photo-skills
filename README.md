# Photo Skills

A growing collection of Codex skills for product photography and creative advertising imagery.

## Skills

| Skill | Path | What it does |
|---|---|---|
| photo-packshot | skills/photo-packshot | Creates accurate product packshots, angle variants, and background variations from real product references. |
| photo-ad-imagery | skills/photo-ad-imagery | Researches photographic references and turns them into distinct creative advertising images. |

Each skill is self-contained under skills/ with its own SKILL.md and references. Add future skills under skills/ using the same photo-* naming pattern.

## Install

Clone this repository, then copy either or both skill folders into the Codex skills directory:

~~~powershell
git clone https://github.com/stanojing-arch/photo-skills.git
Copy-Item -Recurse .\photo-skills\skills\photo-packshot "$env:USERPROFILE\.codex\skills\photo-packshot"
Copy-Item -Recurse .\photo-skills\skills\photo-ad-imagery "$env:USERPROFILE\.codex\skills\photo-ad-imagery"
~~~

Restart or refresh Codex so it can discover the skills.

## 中文说明

这是一个持续扩展的摄影类 Codex skill 集合，当前包含商品静物图和创意广告图两个技能。每个技能独立放在 skills/ 下，后续可继续使用 photo-* 命名添加。

## License

MIT. See LICENSE.
