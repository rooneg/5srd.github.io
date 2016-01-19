---
title: Centipede, Swarm
size: Medium
swarm_size: Tiny
type: Beast
alignment: Unaligned
armor_class: 12
armor_class_descriptor: natural armor
hp: 22
hd: 5
speeds:
  - name: walk
    speed: 20
climb_speeds:
  - name: walk
    speed: 20
ability_scores:
  Strength: 3
  Dexterity: 13
  Constitution: 10
  Intelligence: 1
  Wisdom: 7
  Charisma: 1
damage_resistances:
  - bludgeoning
  - piercing
  - slashing
condition_immunities:
  - charmed
  - frightened
  - grappled
  - paralyzed
  - petrified
  - prone
  - restrained
  - stunned
senses:
  - name: blindsight
    range: 10
challenge: 0.5
special_traits:
  - name: Swarm
    text: The swarm can occupy another creature's space and vice versa, and the swarm can move through any opening large enough for a size Tiny insect. The swarm can't regain hit points or gain temporary hit points.
  - name: Weak Poison
    text: A creature reduced to 0 hit points by a swarm of centipedes is stable but poisoned for 1 hour, even after regaining hit points, and paralyzed while poisoned in this way.
actions:
  - name: Bites
    text: |
      *Melee Weapon Attack:* +3 to hit, reach 0 ft., one target in the swarm's space. *Hit:* 10 (4d4) piercing damage, or 5 (2d4) piercing damage if the swarm has half of its hit points or fewer.
---

This represents a mass of centipedes.

For a more general swarm, see [Insect, Swarm](/monsters/insect-swarm/).
