# new-release-mail-template

Turns approved release facts into a review-ready release announcement email.

It produces:

- **Release Announcement Email:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [New Release Mail Template playbook](https://www.andrewluxem.com/playbooks/new-release-mail-template). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/new-release-mail-template.git
cp -r new-release-mail-template/skills/new-release-mail-template ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r new-release-mail-template/skills/new-release-mail-template ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/new-release-mail-template
/plugin install new-release-mail-template@new-release-mail-template
```

For clients that install from an archive, use the versioned [new-release-mail-template v1.0.0 ZIP](https://www.andrewluxem.com/downloads/new-release-mail-template-v1.0.0.zip).

## Invoke it

```text
Draft the release announcement email from these approved facts
Use the new-release-mail-template skill.
```

Naming the skill is always valid: `use the new-release-mail-template skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/new-release-mail-template/
  assets/release-announcement-email-template.md
  LICENSE.md
  meta.yaml
  references/release-message-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/new-release-mail-template/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/new-release-mail-template/LICENSE.md](skills/new-release-mail-template/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.