# Prologue (Act 0)

This folder contains the prologue design notes and PlantUML diagrams for Act 0.

## Table of Contents

- [Worldbuilding](worldbuilding.puml) — core setting elements to introduce.
- [Game Mechanics](game_mechanics.puml) — onboarding and core mechanics to teach.
- [Story](story.puml) — story beats to establish the hook.
- [Characters](characters.puml) — initial cast and relationships.
- [Prologue Puzzle Flow](eins.puml) — flow of player actions and puzzle outcomes for the prologue. asdf


---

## Worldbuilding

The player is introduced into the world. 
Palmer is not a fish-out-of water character with regards to most things, but he is old and out of touch with the latest technological developments. Jenjen will serve to some extend as introducing concepts via Palmer to the player. But other things will need to be established in different ways. Show, don't tell.

```plantuml
@startuml worldbuilding
title Worldbuilding

package "Worldbuilding" {
	together {

[Introduce World]  --> [Bardo]
[Introduce World]  --> [Homicide]
[Introduce World]  --> [Spaths]
[Introduce World]  --> [Counterwave / Pantha retro]
[FactNet]  --> [Information Control, Censorship]
[Bardo]  --> [Khamma]
[Bardo]  --> [Fractal survival]

[Jenjen] --> [Counterwave / Pantha retro]
[Sunny] --> [Bardo]
[Sunny] --> [Khamma]

	}
}

@enduml
```


## Game Mechanics

This diagram lists the gameplay systems and onboarding priorities to introduce during the prologue.

```plantuml
@startuml game_mechanics
title Game Mechanics

package "Game Mechanics" {
	together {

[Introduce Game Mechanics] --> [Familiarize with BounceBoards]
[Introduce Game Mechanics] --> [Familiarize with chips]
[Introduce Game Mechanics] --> [Familiarize with Lowspace?]
[Introduce Game Mechanics] --> [FactNet]

	}
}

@enduml
```

Summary: Prioritize intuitive, low-risk ways for players to learn these mechanics.

## Story

This section lists the story beats that should be set up in the prologue.

```plantuml
@startuml story
title Story

package "Story" {
	together {

[Kick off Story] --> [Set up mystery and hook]
[Kick off Story] --> [Palmer saves a cat]
[Kick off Story] --> [Transition to new world]
	}
}

@enduml
```

Mystery must be set up to hook the characters and player. In a murder-less world, how can a murder still happen?


## Characters

This diagram lists the initial cast and important relationships introduced in the prologue.

```plantuml
@startuml characters
title Characters

package "Characters" {
	together {

[Introduce Characters]  --> [Palmer]
[Introduce Characters]  --> [Jenjen]
[Introduce Characters]  --> [Boss]
[Introduce Characters]  --> [Bards]
[Bards] --> [Sunny]
[Introduce Characters]  --> [Villain]
[Introduce Characters]  --> [Fake villain]
[Introduce Characters]  --> [veiled Mara]


[Palmer] --> [Save a cat]

	}
}

@enduml
```

Summary: Use the character list to ensure introductions and motivations are clear and consistent.

---

## Prologue Puzzle Flow

This section explains the Prologue Puzzle Flow diagram. It shows how player actions (installing chips,
examining the corpse, acquiring devices) lead to hints and puzzle outcomes (getting Jenjen hints,
finding codes). Use it to validate player progression and pacing.

Diagram file: `act0_puzzles.puml`

![My Diagram Title](./act0_puzzles.puml)

```plantuml
@startuml eins
title ==Prologue Puzzle Flow==
' header __This is the header__
' footer //Confidential - Do not share//

caption This caption is above the diagram

' legend right
' ' ==Legend==
' Alice: Client
' Bob: Server
' end legend

[Install Police Chip] --> [Get Jenjen Hint]
[Examine Corpse] --> [Get Jenjen Hint]


[Acquire Bounce Board Device] --> [Find Code for Counterwave]


' note top of Alice : Client side
' ote top of Bob : Server side

' Alice -> Bob : Request
' Bob --> Alice : Response

@enduml
```

Summary: The puzzle flow diagram captures the essential player actions and their outcomes during the
prologue. Use it to guide puzzle design and ensure necessary signals and clues exist.
