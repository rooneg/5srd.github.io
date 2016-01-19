---
title: Animated Object, Flying Sword
size: Small
type: construct
alignment: unaligned
armor_class: 17
armor_class_descriptor: natural armor
hp: 17
hd: 5
speeds:
  - name: walk
    speed: 0
  - name: fly (hover)
    speed: 50
ability_scores:
  Strength: 12
  Dexterity: 15
  Constitution: 11
  Intelligence: 1
  Wisdom: 5
  Charisma: 1
saving_throw_proficiencies:
  - Dexterity
damage_immunities:
  - poison
  - psychic
condition_immunities:
  - blinded
  - charmed
  - deafened
  - frightened
  - paralyzed
  - petrified
  - poisoned
senses:
  - name: blindsight (blind beyond this radius)
    range: 60
challenge: 0.25
special_traits:
  - name: Antimagic Susceptibility
    text: The armor is incapacitated while in the area of an antimagic field. If targeted by *dispel magic*, the armor must succeed on a Constitution saving throw against the caster's spell save DC or fall unconscious for 1 minute.
  - name: False Appearance
    text: While the sword remains motionless and isn't flying, it is indistinguishable from a normal sword.
actions:
  - name: Longsword
    text: |
      *Melee Weapon Attack:* +3 to hit, reach 5 ft., one target. *Hit:* 5 (1d8 + 1) slashing damage.
---

> **Source:** 5srd adaptation of *Pathfinder Roleplaying Game Bestiary*.
>
> Animated objects come in many sizes and forms, often to the dismay of careless adventurers. Magically brought to permanent pseudo-life by lasting enchantment, these items follow the will of their masters and are often created as guards or sentries in dungeons or castles.
