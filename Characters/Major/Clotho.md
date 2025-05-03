---
cssclasses:
  - notitle
  - character
fighting_style: insert fighting style
combat_ability: insert combat ability
height: insert height
weight: insert weight
pronouns: insert pronouns
likes: like 1, like 2, like 3
dislikes: dislike 1, dislike 2, dislike 3
---
<sub>**A short descriptor**</sub>
# Clotho
<sup>*A punchy tagline.*</sup>
### *Short Info*
``````col
`````col-md
flexGrow=2
===
**Pronouns: ** `= this.pronouns`
**Fighting Style: ** `=this.fighting_style`
**Combat Ability: ** `=this.combat_ability`
	<sup>- Enter additional info here.</sup>
**Height: ** `=this.height`
**Weight: ** `=this.weight`

````col

```col-md
**Likes: ** `$= "<li>" + dv.current().likes.replaceAll(", ", "</li><li>") + "</li>"`
```

```col-md
**Dislikes: ** `$= "<li>" + dv.current().dislikes.replaceAll(", ", "</li><li>") + "</li>"`
```

````
### *Bio*
Add more information here
<br>
`````

`````col-md
flexGrow=1
===
[![[dood3.png]]](dood3.png)
`````

``````



##### ***Personality***
Add info
<br>

##### ***Abilities***
Add info
<br>

### *Relationships*
Add info
<br>

### *Gameplay*
See `$= "[[" + dv.current().file.name + " (Gameplay)]]"`
<br>

### ***Gallery***
```dataviewjs
let imgs = app.vault.getFiles().filter(file => file.path.includes(dv.current().file.name + "_attachments"))

let p = ""; //"````col\n";
for (let i = 0; i < imgs.length; i++) {
	if (i % 5 == 0 && i < imgs.length) {
		if (i !== 0) {
			p += "````\n";
		}
		p += "````col\n";
	}
	
	p += "```col-md\n"
	+ "[![[" + imgs[i].path + "|300]]](" + imgs[i].path + ")\n"
	+ "```\n";
}
p += "````\n";

dv.paragraph(p);
```