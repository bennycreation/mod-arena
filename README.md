# ⚔️ Mod Arena

**Mod Arena** is a Minecraft Java Edition project focused on creating automatic and cinematic battles between different mob factions.

The goal is to go beyond the normal behavior of Minecraft mobs by creating fighters capable of reacting to the situation inside the arena through custom behavioral logic.

The first planned scenario features:

**💀 Skeletons vs 🏹 Pillagers**

---

## 🎯 Project Goal

The mod aims to create battles that are not just a group of mobs spawned in front of each other.

Each fighter may have:

- a role within its team;
- a dynamic target;
- different behaviors;
- special abilities;
- reactions to battle events;
- combat phases;
- sound and particle effects;
- dialogues and narrative events.

The final goal is to create battles that feel like real organized events inside Minecraft.

---

## 🤖 Behavioral AI

The fighters will not be controlled by a language model every game tick.

The mod will use **behavioral AI**, which is much more suitable for real-time Minecraft combat.

A mob may evaluate information such as:

```text
Health
Distance from enemy
Number of allies
Number of enemies
Presence of the leader
Target danger level
Current battle phase
Available abilities
```

and then choose the most appropriate behavior.

Example:

```text
Enemy detected
      │
      ▼
Is health low?
   │       │
  Yes      No
   │       │
Retreat   Attack
            │
            ▼
      Priority target
```

---

## 💀 Skeletons

Skeletons represent one of the two main factions.

Planned behaviors include:

- dynamic target selection;
- ranged combat;
- repositioning;
- evaluation of the most dangerous enemies;
- reactions to allied deaths;
- changes in aggression during the battle.

---

## 🏹 Pillagers

The Pillagers will form an organized team with a hierarchical structure.

Planned features include:

- coordination between team members;
- intelligent target selection;
- offensive and defensive behavior;
- reaction to the leader's death;
- management of different combat phases.

---

## 👑 Pillager Leader

An important part of the scenario will be the **Pillager Leader**.

The leader will be visually recognizable compared to the other members of the team and will have stronger characteristics.

Its role will be to represent the main Pillager fighter and influence the behavior of its faction.

Concept example:

```text
PILLAGER LEADER
│
├── Enemies far away → advance
├── Dangerous enemy → change target
├── Allies in trouble → become more aggressive
├── Low health → defensive strategy
└── Last one alive → final phase
```

---

## 💀 Last Breath

One of the main planned events is the special ability:

# Last Breath

The final Skeleton left alive may automatically activate this ability before being permanently defeated.

During **Last Breath**, the Skeleton may:

- regenerate part of its health;
- receive temporary buffs;
- become more dangerous;
- generate particles and sound effects;
- enter a much harder final phase.

This will create a real final moment in the battle instead of simply eliminating the last remaining mob.

---

## 🎭 Arena Events

The battle will be organized into multiple phases.

A possible complete event:

```text
1. Arena preparation
        ↓
2. Skeleton entrance
        ↓
3. Sound effect
        ↓
4. Pillager entrance
        ↓
5. Leader introduction
        ↓
6. Dialogue between factions
        ↓
7. Battle begins
        ↓
8. Dynamic combat
        ↓
9. Final Skeleton
        ↓
10. "Last Breath" activates
        ↓
11. Final fight
        ↓
12. Victory
```

---

## 🎬 Cinematic Effects

The project plans to use visual and audio elements to make battles more spectacular.

Planned effects include:

- particles;
- ambient sounds;
- unsettling sounds during mob spawning;
- on-screen titles;
- narrative messages;
- dialogue;
- special ability effects;
- victory effects;
- team introductions.

---

## 🏟️ Arena System

The mod will include a dedicated arena management system.

Commands are planned for actions such as:

```text
start a battle
stop a battle
reset the arena
spawn the teams
check the current battle status
```

The final command syntax will be documented once it has been implemented in the code.

---

## 🧠 Project Philosophy

Mod Arena does not aim to create completely pre-scripted battles.

Instead of programming:

```text
Skeleton 1 attacks Pillager 2 after 5 seconds.
```

the goal is to define rules such as:

```text
Find the best enemy target.
Evaluate the danger.
Choose whether to attack, reposition, or defend.
```

This allows two battles to develop differently even when using the same arena.

---

## 🛠️ Technology

The project is intended for:

- **Minecraft Java Edition**
- **Java**
- **Fabric**

The exact Minecraft, Fabric Loader, and Fabric API versions will be specified when the first working build is published.

---

## 📦 Installation

The mod is currently **in development**.

There is no stable release available yet.

Once a build is published, this section will include:

1. required Minecraft version;
2. required Fabric Loader version;
3. required Fabric API version;
4. the mod `.jar` file;
5. installation instructions.

---

## 🗺️ Roadmap

### Phase One

- [ ] Base Fabric project structure
- [ ] Arena system
- [ ] Creation of the two teams
- [ ] Skeleton Fighter AI
- [ ] Pillager Fighter AI
- [ ] Target management

### Phase Two

- [ ] Pillager Leader
- [ ] team behavior
- [ ] battle phases
- [ ] dialogue
- [ ] sound effects
- [ ] particles

### Phase Three

- [ ] **Last Breath** ability
- [ ] final battle phase
- [ ] automatic victory management
- [ ] complete arena reset
- [ ] administrative commands

### Future

The system may later be expanded with:

- new factions;
- new bosses;
- new abilities;
- team battles;
- tournaments;
- customizable arenas;
- different fighter personalities;
- random events;
- spectator mode;
- battle statistics.

---

## 🚧 Project Status

**Mod Arena is currently in the early stages of development.**

The repository will be updated progressively with source code, documentation, and the first playable versions.

---

## 👤 Author

Project developed by **bennycreation**.

---

## 📜 License

The project license has not yet been defined.

Until a `LICENSE` file is added, the code should not be considered automatically available for redistribution or modification.
