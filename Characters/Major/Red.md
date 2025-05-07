---
cssclasses:
  - notitle
  - character
fighting_style: Malnova Tera Batalstilo
combat_ability: "[[Body Augmentation#Improved Tolerance Electrolyte Absorption|Electrolyte]]"
height: 5' 8"
weight: 177 lbs (80 kg)
pronouns: He/Him
faction: "[[Malnova Tero Militia]] (Affiliation Only)"
likes: Even fights, Conflict, Motorized Vehicles
dislikes: Peace, Subversion, Power Imbalances
tags:
  - Immortals
---
<sub>**The Second Immortal Being**</sub>
# Red
<sup>*The fabric of the universe longs for strife.*</sup>
### *Short Info*
``````col
`````col-md
flexGrow=2
===
**Pronouns: ** `= this.pronouns`
**Fighting Style: ** `=this.fighting_style`
**Combat Ability: ** `=this.combat_ability`
	<sup>- Through extensive body augmentation, Red's body can be charged with electricity. His attack power can be greatly amplified by either impacting the enemy or using an Electrolyte injection.</sup>
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
### *Bio*
Red is the second of [[The Four Immortal Beings]], an entity as old as time itself, representing the inherent desire for intelligent life to wage war against one another. He is a master of strategy and martial technique, but intentionally limits himself in order to make engagements more fair/interesting.

At the end of the [[Previous Cycles|previous universe]], the Elioud was be conquered in its entirety by [[White]], who ruled as a God-Emperor. In a shocking turn of events, the Elioud had found a way to survive [[Pale|Pale]]'s [[Placenta of the Fourth|rebirth]], something that had never happened before. Although White and the Elioud gave up captivity of Pale in the process, they were able to retain their empire through the rebirth of the universe. Believing this to be an unfair advantage, Red dedicated his time in the new universe towards the annihilation of White's empire.

<br>
`````

`````col-md
flexGrow=1
===
[![[red.png]]](red.png)
`````

``````

Prior to [[Timeline of 10XX|10XX]], Red became a semi-mythical figure; A rumored sellsword known as 'Vermillion', who could raze entire militias. In reality, Red was using his legend to prompt nations into building stronger and stronger armies, with their ensuing conflict leading to even stronger nations and armies.

With [[Nelchael]]'s arrival and subsequent dedication to humanity's cause, Red found a valuable ally in the war against the Elioud. Initially working in mutual interest, Red found himself in disagreement with Nelchael's plans once Pale was found. Nelchael believed that imprisoning Pale and improving humanity's standard of living would lead to a stronger resistance against White, but Red believed they should kill Pale, establish immortality for humans, and throw their nations into chaos,  turning them into un-killable bloodthirsty warriors. When Nelchael refused, Red coerced a [[Lugh|hero prince]] [[Nona|and]] [[Decima|his]] [[Morta (10XX)|party]] to assassinate Pale.

With Pale dead, Red disappears, leaving Nelchael with seemingly no choice but to overthrow humanity by force, prompting the creation of [[The System]].

In just 1000 years, the System had encompassed the Earth. With most of humanity moved into [[The Empyrean Space]], Red set down his roots in a holdout within the System known as [[Malnova Tero]]. His legend as Vermillion now faded to time, Red slowly built up a new militia, and bided his time.

Prior to 20XX, Red decided it was time. Using his knowledge of the System, he [[Severing of the Connection|severed the Connection]], removing all control the Empyrean had over it. Between the [[Empyrean Space Department of Defense|ESDD]], Malnova Tero, and the [[System Drones]], there would be a new bid for power to control [[Central Administration]] and the System.

In 20XX, Red detects the presence of the [[Placenta of the Fourth]] inside Central Administration. During his investigation, he comes across several [[Anomaly|anomalies]] that pique his interest, including a [[Atropos|pair]] of [[System Drones#*Sentience/Self-Awareness*|sentient]] [[Lachesis|drones]], and a [[Hugh|man with a strange device]] who says he knows something about Pale.

After destroying the Placenta (and Central Administration with it), Red travels to the Empyrean Space, looking to meet with [[Black]]. Red and Black have an honest conversation with each other, with Black revealing his involvement with Atropos' sentience, and Red revealing he was the one who severed the Connection. Upon overhearing this, Atropos (who was being held captive by Black), kills Red, sending him back to the System.

Red returns to Malnova Tero, where he waits for his next move.
<br>

##### ***Personality***
Red isn't very expressive. He very rarely shows emotion on his face, and even when it does, it is questionable whether or not he is doing so just for show. A quiet man, Red tends to keep his conversations short and direct, opting to let his fists do the talking when dealing with potential enemies.

He does seem to get some amusement from having a good sparring partner, or when his plans go in his favor. He also seems to show some softness when interacting with his wife, [[Laila]], as well as his daughter, [[Maeve]]. However, as Maeve grows older, she begins to question her father's sincerity.

<br>

##### ***Abilities***
Add info
<br>

### *Relationships*
Add info
<br>

### *Gameplay*
*Main Article: `$= "[[" + dv.current().file.name + " (Gameplay)]]"`*
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