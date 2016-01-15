---
title: Snake, Poisonous, Swarm
size: Medium
swarm_size: Tiny
type: Beast
alignment: Unaligned
ac: 14
hp: 36
hd: 8
hd_size: 8
speeds:
  - name: walk
    speed: 30
  - name: swim
    speed: 30
str: 8
dex: 18
con: 11
int: 1
wis: 10
cha: 3
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
  - name: Blindsight
    range: 10
challenge: 2
special_traits:
  - name: Swarm
    text: The swarm can occupy another creature's space and vice versa, and the swarm can move through any opening large enough for a size Tiny snake. The swarm can't regain hit points or gain temporary hit points.
actions:
  - name: Bites
    text: >
      *Melee Weapon Attack:* +6 to hit, reach 0 ft., one creature in the swarm's space. *Hit:* 7 (2d6) piercing damage, or 3 (1d6) piercing damage if the swarm has half of its hit points or fewer. The target must make a DC 10 Constitution saving throw, taking 14 (4d6)  poison damage on a failed save, or half as much damage on a successful one.
---
