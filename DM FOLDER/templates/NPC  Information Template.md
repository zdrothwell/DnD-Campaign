---
AssociatedGroup: 
Gender: 
Race: 
Age: 
Class: 
Alignment: 
Character-Role: 
Location: 
AssociatedGroup: 
NoteIcon: npc
---

<% tp.file.title %>
<% await tp.file.move("DM FOLDER/Mechanics/Non-Player Characters/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewNPC");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter NPC Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

> [!infobox]
> # `=this.file.name`
> ![[ImagePlaceholder.png|cover hsmall]]
> [[ImagePlaceholder.png|Show To Players]]
> ###### Basic Information
> Type |  Stat |
> ---|---|
> Home | `=this.Location` |
> Group | `=this.AssociatedGroup` |
> Sex | `=this.gender` |
> Race | `=this.race` |
> Age | `=this.age` |
> Condition | Healthy |
> ###### Rules Info
> Type |  Stat |
> ---|---|
> Alignment | `=this.alignment` |
> Class | `=this.class` |
> Character Role | `=this.character-role` |

# `=this.file.name`
## Profile

<% tp.file.cursor() %>
**<Add description here, extend it with AI Text Generator using Ctrl J>**

> [!info] Statblock
> ```statblock
> name: Individual
> monster: Commoner
> columns: 1
> ```
