# Assisticant Skills

A set of [Claude Code](https://claude.com/claude-code) skills for working with
[Assisticant](https://github.com/michaellperry/Assisticant), a dependency
tracking library for .NET. Assisticant is available on
[NuGet](https://www.nuget.org/packages/Assisticant); its source code is at
<https://github.com/michaellperry/Assisticant>.

Each skill is a folder containing a `SKILL.md` file that teaches an agent how
to use part of the library.

## Skills

| Skill | Description |
| --- | --- |
| [`assisticant-source-generators`](assisticant-source-generators/SKILL.md) | Guidance on the `[Observable]`, `[Computed]`, `[NotifyPropertyChanged]`, and `[Command]` source-generator prototype: which attribute to use, and what each platform (WPF, UWP, Android, iOS, MAUI) needs. |

## Installation

### With OpenSkills

Install all of the skills in this repository using
[OpenSkills](https://github.com/numman-ali/openskills):

```bash
npx openskills install assisticant/skills
```

### Manually

Copy or symlink a skill folder into your skills directory.

- Personal (all projects): `~/.claude/skills/<skill-name>/`
- Project (shared with your team): `<project>/.claude/skills/<skill-name>/`

For example:

```powershell
Copy-Item -Recurse assisticant-source-generators $HOME\.claude\skills\
```

Claude loads a skill automatically when your request matches its description.

## Contributing

To add a skill, create a new folder with a `SKILL.md` that has `name` and
`description` frontmatter, then list it in the table above.

## License

[MIT](LICENSE)
