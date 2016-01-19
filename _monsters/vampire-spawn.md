---
title: Vampire Spawn
size: Medium
type: undead
alignment: neutral evil
armor_class: 15
armor_class_descriptor: natural armor
hp: 82
hd: 11
speeds:
  - name: walk
    speed: 30
ability_scores:
  Strength: 16
  Dexterity: 16
  Constitution: 16
  Intelligence: 11
  Wisdom: 10
  Charisma: 12
saving_throw_proficiencies:
  - Dexterity
  - Wisdom
skills:
  - name: Perception
    bonus: 3
  - name: Stealth
    bonus: 6
damage_resistances:
  - necrotic
  - bludgeoning, piercing, and slashing from nonmagical attacks
senses:
  - name: darkvision
    range: 60
languages:
  - the languages it knew in life
challenge: 5
special_traits:
  - name: Regeneration
    text: The vampire regains 10 hit points at the start of its turn if it has at least 1 hit point and isn't in sunlight or running water. If the vampire takes radiant damage or damage from holy water, this trait doesn't function at the start of the vampire's next turn.
  - name: Spider Climb
    text: The vampire can climb difficult surfaces, including upside down on ceilings, without needing to make an ability check.
  - name: Vampire Weaknesses
    text: |
      The vampire has the following flaws:

      - *Forbiddance.* The vampire can't enter a residence without an invitation from one of the occupants.
      - *Harmed by Running Water.* The vampire takes 20  acid damage when it ends its turn in running water.
      - *Stake to the Heart.* The vampire is destroyed if a piercing weapon made of wood is driven into its heart while it is incapacitated in its resting place.
      - *Sunlight Hypersensitivity.* The vampire takes 20  radiant damage when it starts its turn in sunlight. While in sunlight, it has disadvantage on attack rolls and ability checks.
actions:
  - name: Multiattack
    text: The vampire makes two attacks, only one of which can be a bite attack.
  - name: Claws
    text: |
      *Melee Weapon Attack:* +6 to hit, reach 5 ft., one creature. *Hit:* 8 (2d4 + 3) slashing damage. Instead of dealing damage, the vampire can grapple the target (escape DC 13).
  - name: Bite
    text: |
       *Melee Weapon Attack:* +6 to hit, reach 5 ft., one willing creature, or a creature that is grappled by the vampire, incapacitated, or restrained. *Hit:* 6 (1d6 + 3) piercing damage plus 7 (2d6) necrotic damage. The target's hit point maximum is reduced by an amount equal to the necrotic damage taken, and the vampire regains hit points equal to that amount. The reduction lasts until the target finishes a long rest. The target dies if this effect reduces its hit point maximum to 0.
---
