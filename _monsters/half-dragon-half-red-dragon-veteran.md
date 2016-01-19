---
title: Half-Dragon, Half-Red Dragon Veteran
size: Medium
type: humanoid
tags:
  - human
alignment: any
armor_class: 18
armor_class_descriptor: plate
hp: 65
hd: 10
speeds:
  - name: walk
    speed: 30
ability_scores:
  Strength: 16
  Dexterity: 13
  Constitution: 14
  Intelligence: 10
  Wisdom: 11
  Charisma: 10
skills:
  - name: Athletics
    bonus: 5
  - name: Perception
    bonus: 2
damage_resistances:
  - fire
senses:
  - name: blindsight
    range: 10
  - name: darkvision
    range: 60
languages:
  - Common
  - Draconic
challenge: 5
actions:
  - name: Multiattack
    text: |
       The veteran makes two longsword attacks. If it has a shortsword drawn, it can also make a shortsword attack.
  - name: Longsword
    text: |
       *Melee Weapon Attack:* +5 to hit, reach 5 ft., one target. *Hit:* 7 (1d8 + 3) slashing damage, or 8 (1d10  + 3) slashing damage if used with two hands.
  - name: Shortsword
    text: |
       *Melee Weapon Attack:* +5 to hit, reach 5  ft., one target. *Hit:* 6 (1d6 + 3) piercing damage.
  - name: Heavy Crossbow
    text: |
       *Ranged Weapon Attack:* +3 to hit, range 100/400 ft., one target. *Hit:* 6 (1d10 + 1) piercing damage.
  - name: Fire Breath (Recharge 5--6)
    text: |
       The veteran exhales fire in a 15-foot cone. Each creature in that area must make a DC 15 Dexterity saving throw, taking 24 (7d6) fire damage on a failed save, or half as much damage on a successful one.
---
