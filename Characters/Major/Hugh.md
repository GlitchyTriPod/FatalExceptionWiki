---
cssclasses:
  - notitle
  - character
fighting_style: Improvised Technique, based on ESDD Training
combat_ability: "[[Cybermessiah]]"
height: 5' 10" (177 cm)
weight: 190 lbs (86 kg)
pronouns: He/Him
faction: "[[Empyrean Space Department of Defense|ESDD]]"
likes: Roughhousing, Clean laundry, The goodie bars in ESDD field rations
dislikes: Loneliness, Riddles, Sand
---
<sub>**Artificial Human, ESDD Operator \#5762**</sub>
# Hugh
<sup>*The light of optimism in the face of pure darkness.*</sup>
### *Short Info*
``````col
`````col-md
flexGrow=2
===
**Pronouns: ** `= this.pronouns`
**Fighting Style: ** `=this.fighting_style`
**Combat Ability: ** `= this.combat_ability`
	<sup>- A hulking weapon that can fire out devastating bolts of energy. Due to its long charging period, Hugh more often uses it as a bludgeoning tool.</sup>
**Faction: ** `=this.faction`
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

`````

`````col-md
flexGrow=1
===
[![[hugh.png]]](hugh.png)
`````

``````

### *Bio*
Hugh is an [[Artificial Humans|Artificial Human]] created by the Epyrean Space Department of Defense (ESDD). Trained from gestation to be a soldier, he had basic training -- CQC and survival techniques -- implanted into his mind using a VR training regiment. After the [[Severing of the Connection]] the ESDD [[Pale Ops]] R&D team developed the [[Cybermessiah]], a weapon which required a mental link with its wielder. For unknown reasons, the Cybermessiah chose to be with Hugh.

Following the device's cryptic instructions, Hugh enters [[The System]] with his platoon in order to re-establish [[The Connection]], but are quickly executed by [[Atropos]] and the [[System Drones#E-Class|E-Class drones]]. In a moment of hesistation, Atropos lets Hugh fall into the System's depths instead of killing him immediately. After falling for around 48 hours, Hugh eventually hits the [[Solid Material Plane]]. The Cybermessiah establishes a new [[Tether]] before Hugh impacts the ground, where he [[Death and Immortality|dies for the first time]].

After recovering at the new tether point, Hugh decides to complete the mission on his own. After making his way up to [[Central Administration (Location)|Central Administration]] (and dying multiple times along the way), Hugh learns that [[Red]] was the one who severed The Connection, albeit for unknown reasons. After defeating Red, Hugh connects the Cybermessiah to Central Administration in order to re-establish the Connection. However, due to the mental like he has with the Cybermessiah, Hugh's consciousness is also pulled inside Central Administration.

Inside of the Connection's cyberspace, the Cybermessiah presents itself to Hugh as a being known as [[Pale (Tragedy)|Pale<Tragedy>]], a copy of the [[Pale|consciousness that The System was based on]]. Another being, [[Pale (Comedy)|Pale<Comedy>]], also appears. Pale\<Comedy> claims to be the original consciousness of the System, and the manifestation of [[The System's Will]]. After the two copies of Pale argue over how the System should be managed, Hugh is tasked with overseeing the creation of a new copy of Pale, one that could be an unbiased judge against the world. Believing that an unbiased observer could see the "inherent goodness" in the Empyrean Space, he accepts the task.

Returning to the System, Hugh finds Central Administration in ruins (presumably destroyed by Red). As he proceeds towards his next destination he is intercepted by [[Plasma]], who was sent to retrieve the Cybermessiah. A chase ensues, with Hugh just barely able to finish creating the [[Sys._Pseudo(Pale)|new Pale copy]] before being incapacitated.

Afterwards, Hugh becomes an asset of the ESDD Pale Ops. Although the Pale Ops cannot trust Hugh with keeping their secrets, they cannot get rid of him as the wielder of the Cybermessiah. As such, he is sent into the System on numerous missions, working alongside the likes of [[Black]], [[Unnamed (Magical Girl) Group]], and -- most notably -- becoming cellmates with [[Morta]].

##### ***Personality***
Hugh is the definition of an optimist, the kind of person that believes that good will ultimately prevail over evil. As he is an artificial human created by the ESDD, his wider knowledge of Empyrean society and politics is very small. As a result, his optimistic outlook tends to come off as childish. Hugh continues to confidently stick to his beliefs, even when confronted with the reality of both the System and the Empyrean space.

While Hugh takes his mission seriously, his natural disposition is lighthearted and laid-back. He tends to get under the skin of his opponents by playfully teasing them, but never outright insulting them.  What he lacks in intelligence and experience, Hugh makes up for in playfulness and sheer willpower.

<br>

##### ***Abilities***
Add info
<br>

### *Relationships*
Add info
<br>

### *Gameplay*
*Main Article:  `$= "[[" + dv.current().file.name + " (Gameplay)]]"`*
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