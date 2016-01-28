---
title: Goblin, Spider-Eye, Shaman
source: |
  [*Gauntlet of Spiragos*](http://www.drivethrurpg.com/product/171523/Gauntlet-of-Spiragos-5E-OGL-adventure)
size: Small
type: monstrosity
alignment: neutral evil
armor_class: 14
armor_class_descriptor: natural armor
hp: 14
hd: 4
speeds:
  - name: walk
    speed: 30
  - name: climb
    speed: 20
ability_scores:
  Strength: 9
  Dexterity: 13
  Constitution: 10
  Intelligence: 8
  Wisdom: 13
  Charisma: 9
skills:
  - name: Perception
    bonus: 5
  - name: Stealth
    bonus: 5
damage_resistances:
  - poison
senses:
  - name: darkvision
    range: 60
languages:
  - Goblin
  - Undercommon
challenge: 0.5
special_traits:
  - name: Keen Sight
    text: The shaman has advantage on Wisdom (Perception) checks that rely on sight.
  - name: Nimble Escape
    text: The shaman can take the Disengage or Hide action as a bonus action on each of her turns.
  - name: Spellcasting
    text: |
      The shaman is a 2nd-level spellcaster. Her spellcasting ability is Wisdom (spell save DC 11, +3 to hit with spell attacks). The shaman has the following spells prepared:

      - Cantrips (at will): [*acid splash*](/spells/acid-splash/), [*mending*](/spells/mending/)
      - 1st level (3 slots): [*faerie fire*](/spells/faerie-fire/), [*healing word*](/spells/healing-word/), [*speak with animals*](/spells/speak-with-animals/)
actions:
  - name: Multiattack
    text: The spider-eye goblin makes two claw attacks. If both claw attacks hit the same target, the goblin can then make one bite attack against that target.
  - name: Claw
    text: |
      *Melee Weapon Attack:* +3 to hit, reach 5 ft., one target. *Hit:* 3 (1d4+1) slashing damage.
  - name: Bite
    text: |
      *Melee Weapon Attack:* +3 to hit, reach 5 ft., one target. *Hit:* 3 (1d4+1) piercing damage, and the target must make a DC 10 Constitution saving throw, taking 2 (1d4) poison damage on a failed save, or half as much damage on a successful one. If this poison damage reduces the target to 0 hit points, the target is stable but poisoned for 1 hour, even after regaining hit points, and is paralyzed while poisoned in this way.
  - name: Dart
    text: |
      *Ranged Weapon Attack:* +3 to hit, range 20/60 ft., one target. *Hit:* 3 (1d4+1) piercing damage.
---

See the [spider-eye goblin](/monsters/goblin-spider-eye/) entry for lore and behavior information.
