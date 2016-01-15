---
title: Panther
size: Medium
type: Beast
alignment: Unaligned
ac: 12
hp: 13
hd: 3
speeds:
  - name: walk
    speed: 50
climb_speeds:
  - name: walk
    speed: 40
str: 14
dex: 15
con: 10
int: 3
wis: 14
cha: 7
skills:
  - name: Perception
    bonus: 4
  - name: Stealth
    bonus: 6
challenge: 0.25
special_traits:
  - name: Keen Smell
    text: The panther has advantage on Wisdom  (Perception) checks that rely on smell.
  - name: Pounce
    text: If the panther moves at least 20 feet straight toward a creature and then hits it with a claw attack on the same turn, that target must succeed on a DC 12 Strength saving throw or be knocked prone. If the target is prone, the panther can make one bite attack against it as a bonus action.
actions:
  - name: Bite
    text: >
      *Melee Weapon Attack:* +4 to hit, reach 5 ft., one target. *Hit:* 5 (1d6 + 2) piercing damage.
  - name: Claw
    text: >
      *Melee Weapon Attack:* +4 to hit, reach 5 ft., one target. *Hit:* 4 (1d4 + 2) slashing damage.
---
