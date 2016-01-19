---
title: Rat, Swarm
size: Medium
swarm_size: Tiny
type: Beast
alignment: Unaligned
armor_class: 10
hp: 24
hd: 7
speeds:
  - name: walk
    speed: 30
ability_scores:
  Strength: 9
  Dexterity: 11
  Constitution: 9
  Intelligence: 2
  Wisdom: 10
  Charisma: 3
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
  - name: darkvision
    range: 30
challenge: 0.25
special_traits:
  - name: Keen Smell
    text: The swarm has advantage on Wisdom (Perception) checks that rely on smell.
  - name: Swarm
    text: The swarm can occupy another creature's space and vice versa, and the swarm can move through any opening large enough for a size Tiny rat. The swarm can't regain hit points or gain temporary hit points.
actions:
  - name: Bites
    text: |
      *Melee Weapon Attack:* +2 to hit, reach 0 ft., one target in the swarm's space. *Hit:* 7 (2d6) piercing damage, or 3 (1d6) piercing damage if the swarm has half of its hit points or fewer.
---
