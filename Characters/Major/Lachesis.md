---
cssclasses:
  - notitle
  - character
fighting_style: O-Class Defensive Strategies - Nonstandard Augmentations
combat_ability: Anti-Gravitational Propulsion (AGP) Sub-Drones
height: 6' 3" (190 cm)
weight: 237 lbs (107 kg)
pronouns: She/Her
faction: "[[Central Administration]]"
likes: Ambition, Her precious “Sisters”, Experimentation
dislikes: Disobedience, Societal Norms, Boredom
---
<sub>**O-Class Administration Drone, Serial Number \#O0303**</sub>
# Lachesis
<sup>*Where the thread should be cut lies the potential for it to instead split.*</sup>
### *Short Info*
``````col
`````col-md
flexGrow=2
===
**Pronouns: ** `= this.pronouns`
**Fighting Style: ** `=this.fighting_style`
**Combat Ability: ** `=this.combat_ability`
	<sup>- Four miniature drone units that provide Lachesis with unparalleled range and stopping power.</sup>
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
System Drone \#O0303 (unit model name "Lachesis") is an [[System Drones#O-Class|O-Class System Drone]] that was designed for high-level Operations Management at [[Central Administration (Location)|Central Administration]]. Immediately after [[Severing of the Connection|the Connection was severed]], the [[Pale (Comedy)|conscious entity that ran the System]] implanted new procedures into the processes of all operational O-Class drones. As a result, all O-Class drones were destroyed, with Lachesis being the only survivor.

<br>
`````

`````col-md
flexGrow=1
===
[![[lach.png]]](lach.png)
`````

``````

With Pale\<Comedy>'s new instruction set, Lachesis became [[System Drones#*Sentience/Self-Awareness*|sentient]]. Along with this newfound self-awareness, she found herself with knowledge about a machine known as the [[Placenta of the Fourth]], not understanding how she knew of the schematics, but understanding that it could bestow unbelievable power unto her. Now a defect (and with her [[Drone Technology#Personality Mimesis Drive| Personality Mimesis Drive]] damaged), Lachesis obsessively pursued the construction of the Placenta, alongside [[Lachesis#Abilities|installing off-model drone parts onto herself]] and creating [[System Drones#Haywires|Haywires]] from the remains of her fellow O-Class drones. 

As a result of her actions, Lachesis provokes conflict between her, [[Atropos]], [[Hugh]], and [[Red]]. After Atropos realizes that Lachesis is a defect (and that the Placenta is an existential threat to [[The System]]), Atropos destroys her. With a momentary agreement, Atropos allows Red to destroy the Placenta, which takes out most of Central Administration with it. Because of Central Administration's destruction, Lachesis is unable to be completely rebuilt.

Immobile (and full of rage) Lachesis explains to Atropos that in order for the System to continue existing, there must be a Central Administration, and in order to create a new Central Administration, there must be an O-Class to operate it. Atropos disagrees, leaving Lachesis to rot.

Luckily for her, a [[Clotho|wandering C-Class drone]] happens to find her. Taking pity on Lachesis, Clotho transports her across the System, where she is eventually rebuilt. Refurbished, Lachesis vows to take revenge on the humans for their meddlesome behavior. Using the last of her authority (and preying on Clotho's emotions), Lachesis directs the C-Class Drones to begin excavating the [[Threshold Obfuscation Field]], and preparing the architecture and machinery needed to [[The Drowning of the Empyrean Space|completely submerge]] the entrance to [[The Empyrean Space]].

Although Lachesis fails to completely destroy the Empyrean Space, she deals a huge blow to the stability of Empyrean society. As the ESDD and the [[Nelchael|Empyrean]] [[Adrian|leadership]] scramble to regain control, Lachesis proclaims herself as the rightful ruler of the System, vowing to rebuild the Placenta.
<br>

##### ***Personality***
As an O-Class drone, Lachesis has a [[Drone Technology#Personality Mimesis Drive|Personality Mimesis Drive]] installed, naturally allowing her a wider range of expression. Under normal conditions, the O-Class drones are programmed with emotional limiters, preventing personality traits like obsession, panic, or hysteria. As Lachesis is a defect, she is prone to extreme emotions.

While communicating remotely, Lachesis comes off as somewhat quirkier than the average O-Class -- sometimes breaking into fits of giggling -- but retains most of the politeness that the O-Class is known for. In-person, Lachesis' perverted nature is more apparent; Her polite requests turn into authoritative commands, her giggles break into maniacal laughter, and her fondness for her fellow drone "sisters" steers towards overt lechery.

Lachesis revels in the defiance of her intended programming, the breaking of purpose and societal expectation giving her some kind of high. She takes immense pleasure in "disassembling" her enemies, and does so with a smile on her face.

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