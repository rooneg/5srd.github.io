---
title: Boar
size: Medium
type: Beast
alignment: Unaligned
ac: 11
natural_armor: true
hp: 11
hd: 2
hd_size: 8
speeds:
  - name: walk
    speed: 40
str: 13
dex: 11
con: 12
int: 2
wis: 9
cha: 5
challenge: 0.25
special_traits:
  - name: Charge
    text: If the boar moves at least 20 feet straight toward a target and then hits it with a tusk attack on the same turn, the target takes an extra 3 (1d6)  slashing damage. If the target is a creature, it must succeed on a DC 11 Strength saving throw or be knocked prone.
  - name: Relentless (Recharges after a Short or Long Rest)
    text: If the boar takes 7 damage or less that would reduce it to 0 hit points, it is reduced to 1 hit point instead.
actions:
  - name: Tusk
    text: >
      *Melee Weapon Attack:* +3 to hit, reach 5 ft., one target. *Hit:* 4 (1d6 + 1) slashing damage.
---
