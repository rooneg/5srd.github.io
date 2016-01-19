---
title: Spider, Giant, Wolf
size: Medium
type: Beast
alignment: Unaligned
armor_class: 13
hp: 11
hd: 2
speeds:
  - name: walk
    speed: 40
climb_speeds:
  - name: walk
    speed: 40
ability_scores:
  Strength: 12
  Dexterity: 16
  Constitution: 13
  Intelligence: 3
  Wisdom: 12
  Charisma: 4
skills:
  - name: Perception
    bonus: 3
  - name: Stealth
    bonus: 7
senses:
  - name: blindsight
    range: 10
  - name: darkvision
    range: 60
challenge: 0.25
special_traits:
  - name: Spider Climb
    text: The spider can climb difficult surfaces, including upside down on ceilings, without needing to make an ability check.
  - name: Web Sense
    text: While in contact with a web, the spider knows the exact location of any other creature in contact with the same web.
  - name: Web Walker
    text: The spider ignores movement restrictions caused by webbing.
actions:
  - name: Bite
    text: |
      *Melee Weapon Attack:* +3 to hit, reach 5 ft., one creature. *Hit:* 4 (1d6 + 1) piercing damage, and the target must make a DC 11 Constitution saving throw, taking 7 (2d6) poison damage on a failed save, or half as much damage on a successful one. If the poison damage reduces the target to 0 hit points, the target is stable but poisoned for 1 hour, even after regaining hit points, and is paralyzed while poisoned in this way.
---
