---
cssclasses:
  - notitle
  - character
fighting_style: E-Class Drone Martial Techniques, High Mobility
combat_ability: "[[Drone Technology#Capability Enhancement Thrusters|Capability Enhancement Thrusters]] (CETs)"
height: 5' 5" (165 cm)
weight: 330 lbs (149 kg)
pronouns: It/Its*
faction: "[[System Drones]]"
likes: Direction, Purpose, Maintaining System Integrity
dislikes: Free will, Humanity, Anomalies
tags:
 - Drones
---
<sub>**E-Class Specialized Combat Drone, Serial Number \#E9924**</sub>
# Atropos
<sup>*A yearning for the thoughtlessness of bare metal.*</sup>
### *Short Info*
``````col
`````col-md
flexGrow=2
===
**Pronouns: ** `= this.pronouns`
	<sup>\* Usage of 'They/Them' is appropriate in most cases. Read the section on [[#Personality]] for more information.</sup>
**Fighting Style: ** `=this.fighting_style`
**Combat Ability: ** `=this.combat_ability`
	<sup>- Using embedded propulsion units, Atropos' mobility and attack power is greatly augmented.</sup>
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
[![[atro.png]]](atro.png)
`````

``````

### *Bio*
System Drone \#E9924 (unit model name "Atropos") is an [[Drone Technology#E-Class|E-Class System Drone]] that was designated as a specialized combat unit through [[Drone Technology#Capability Enhancement Thrusters| CET]] upgrades. As a result of [[Black]]'s interference with [[The System]] under [[Central Administration]]'s nose prior to [[Severing of the Connection|the Connection being severed]], Atropos was constructed as a defect with [[Drone Technology#*Sententience/Self-Awareness*|sentience]].

Following orders from [[Central Administration]], Atropos is commanded to execute (destroy) all [[Anomaly|Anomalies]]. Upon the completion of their first task after construction -- the execution of [[Hugh]] after his [[Empyrean Space Department of Defense|ESDD]] platoon came through [[The Threshold]] -- Atropos became cognizant of their sentience.

Over the course of [[Fatal Exception]], Atropos learns that Central Administration is compromised. With the Connection being severed, and the [[Lachesis|last O-Class drone]] also a defect, there is no real authority left to enact [[The System's Will]]. Following orders from the damaged Central Administration, Atropos attempts to invade the [[The Empyrean Space]] alongside their fellow E-Class drones. However, the invasion is quickly quashed, with Atropos being captured by Black after being severely damaged.

In captivity, Black reveals himself to Atropos as the cause of their sentience. In the event that the ESDD lost control of the System, a unit could be created that could help the ESDD restore control. As an appeal to Atropos' ethos, Black explains that the System was created in humanity's interest; That the proper course of action would be for Atropos to ignore their current prime directive, and work towards restoring the Connection. Atropos instead doubles down, ignoring Black's plea as he is not an arbiter of the System's Will, but is -- categorically -- an Anomaly. In response, Black begrudgingly makes a copy of Atropos' consciousness in order to create a version of them that would act in service to the ESDD. This copy eventually lands in the hands of [[Adrian|ESDD Lead Scientist Adrian]], who uses it as the basis for [[Morta]]'s creation.

Atropos' damaged body would remain in Black's safe house in an extended recovery mode. It is only after [[The Drowning of the Empyrean Space]] that Atropos is able to return to the System, being washed back through the threshold during the flood. The ESDD, now having research settlements outside of the [[Threshold Obfuscation Field]], is able to recover their body and repair it as means of researching the psyche of defected drones. Having pity on Atropos, Black enables their escape.

Now back in the System, Atropos finds themselves without orders. Without any authority to speak the System's Will, Atropos has no direction. Accepting at least some part of their sentience, Atropos decided that the only way forward is to re-implement the System's Will themselves -- To rebuild a new Central Authority, free from defects, and to execute all Anomalies.

<br>

#### ***Personality***
As an E-Class drone, Atropos does not have a [[Drone Technology#Personality Mimesis Drive|Personality Mimesis Drive]] installed, resulting in their overall personality to be somewhat flat. However, after their self-awareness manifests, they begin showing signs of internal conflict and emotion. Atropos desires, above all else, to execute the will of The System (with orders typically coming down from Central Administration). They view their actions not as self-fulfillment, but as fulfillment of their purpose (literally, doing what they were built to do). Any emotion that may be elicited from their own actions considered an obstacle to fulfilling their purpose.

Atropos primarily exhibits anger, frustration, and self-loathing, often resorting to physical violence when their thought patterns are challenged.

Although self-awareness inflicts stress upon them, Atropos' sentience is what allows them to push through their negative thoughts in order to re-implement The System's will.

*Regarding "It/Its" Pronouns*
Atropos is not accepting of human identity; They do not view themselves as Human, a person, or as a living being. As such, they would prefer being referenced to as "It" over "They/Them". However, in casual conversation (and for ease of communication both in-universe and in real life) "They/Them" can be used, to Atropos' ire. Additionally, Atropos typically refers to themselves using "This Unit" over personal identifiers like "I/Me", although this begins to slip as their self-awareness grows.
<br>

#### ***Abilities***
Add info
<br>

#### ***Relationships***
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