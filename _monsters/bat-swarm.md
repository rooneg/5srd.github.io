---
title: Bat, Swarm
size: Medium
swarm_size: Tiny
type: Beast
alignment: Unaligned
ac: 12
hp: 22
hd: 5
hd_size: 8
speeds:
  - name: walk
    speed: 0
  - name: fly
    speed: 30
str: 5
dex: 15
con: 10
int: 2
wis: 12
cha: 4
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
    range: 60
challenge: 0.25
special_traits:
  - name: Echolocation
    text: The swarm can't use its blindsight while deafened.
  - name: Keen Hearing
    text: The swarm has advantage on Wisdom  (Perception) checks that rely on hearing.
  - name: Swarm
    text: The swarm can occupy another creature's space and vice versa, and the swarm can move through any opening large enough for a size Tiny bat. The swarm can't regain hit points or gain temporary hit points.
actions:
  - name: Bites
    text: >
      *Melee Weapon Attack:* +4 to hit, reach 0 ft., one creature in the swarm's space. *Hit:* 5 (2d4) piercing damage, or 2 (1d4) piercing damage if the swarm has half of its hit points or fewer.
---
