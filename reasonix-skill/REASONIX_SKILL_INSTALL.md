# CLI-Anything for Reasonix — Native Skill Definition

This file can be installed directly into Reasonix via the `install_skill` tool:

```
install_skill({
  name: "cli-anything",
  description: "Build, refine, test, or validate a CLI-Anything harness for any GUI application or source repository.",
  body: "<contents of SKILL.md>",
  runAs: "subagent",
  scope: "global"
})
```

When run as a subagent, the skill spawns an isolated Reasonix sub-agent that
has access to all standard tools (bash, read_file, write_file, edit_file, etc.)
and follows the CLI-Anything 7-phase methodology without polluting the parent
session's context.
