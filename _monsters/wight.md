---
title: Wight
size: Medium
type: undead
alignment: neutral evil
armor_class: 14
armor_class_descriptor: studded leather
hp: 45
hd: 6
speeds:
  - name: walk
    speed: 30
ability_scores:
  Strength: 15
  Dexterity: 14
  Constitution: 16
  Intelligence: 10
  Wisdom: 13
  Charisma: 15
skills:
  - name: Perception
    bonus: 3
  - name: Stealth
    bonus: 4
damage_resistances:
  - necrotic
  - bludgeoning, piercing, and slashing from nonmagical attacks that aren't silvered
damage_immunities:
  - poison
condition_immunities:
  - exhaustion
  - poisoned
senses:
  - name: darkvision
    range: 60
languages:
  - the languages it knew in life
challenge: 3
special_traits:
  - name: Sunlight Sensitivity
    text: While in sunlight, the wight has disadvantage on attack rolls, as well as on Wisdom (Perception) checks that rely on sight.
actions:
  - name: Multiattack
    text: The wight makes two longsword attacks or two longbow attacks. It can use its Life Drain in place of one longsword attack.
  - name: Life Drain
    text: |
      *Melee Weapon Attack:* +4 to hit, reach 5 ft., one creature. *Hit:* 5 (1d6 + 2) necrotic damage. The target must succeed on a DC 13 Constitution saving throw or its hit point maximum is reduced by an amount equal to the damage taken. This reduction lasts until the target finishes a long rest. The target dies if this effect reduces its hit point maximum to 0.

      A humanoid slain by this attack rises 24 hours later as a [zombie](/monsters/zombie-humanoid/) under the wight's control, unless the humanoid is restored to life or its body is destroyed.  The wight can have no more than twelve zombies under its control at one time.
  - name: Longsword
    text: |
      *Melee Weapon Attack:* +4 to hit, reach 5 ft., one target. *Hit:* 6 (1d8 + 2) slashing damage, or 7 (1d10  + 2) slashing damage if used with two hands.
  - name: Longbow
    text: |
      *Ranged Weapon Attack:* +4 to hit, range  150/600 ft., one target. *Hit:* 6 (1d8 + 2) piercing damage.
---
