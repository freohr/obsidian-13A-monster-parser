---
level: {{VALUE:level}}
role: {{VALUE:role}}
type: {{VALUE:type}}
strength: {{VALUE:size}}
tags: ["13A/Bestiary/{{VALUE:type}}", "13A/Monsters/Faction/{{VALUE:faction}}", "13A/Monsters/Role/{{VALUE:role}}", "13A/Monsters/Strength/{{VALUE:size}}"]
alias:
  - {{VALUE:name}}
---
```statblock
layout: Basic 13th Age Monster Layout
columns: 1
{{VALUE:fullBlock}}
```
```js quickadd
const prompter = new customJS.Parser13AMonster.QuickAddPrompter(this);
this.variables["fullBlock"] = await prompter.promptMinimalistParser();
```