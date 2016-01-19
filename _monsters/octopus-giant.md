---
title: Octopus, Giant
size: Large
type: Beast
alignment: Unaligned
armor_class: 11
hp: 52
hd: 8
speeds:
  - name: walk
    speed: 10
  - name: swim
    speed: 60
ability_scores:
  Strength: 17
  Dexterity: 13
  Constitution: 13
  Intelligence: 4
  Wisdom: 10
  Charisma: 4
skills:
  - name: Perception
    bonus: 4
  - name: Stealth
    bonus: 5
senses:
  - name: darkvision
    range: 60
challenge: 1
special_traits:
  - name: Hold Breath
    text: While out of water, the octopus can hold its breath for 1 hour.
  - name: Underwater Camouflage
    text: The octopus has advantage on Dexterity (Stealth) checks made while underwater.
  - name: Water Breathing
    text: The octopus can breathe only underwater.
actions:
  - name: Tentacles
    text: |
      *Melee Weapon Attack:* +5 to hit, reach 15 ft., one target. *Hit:* 10 (2d6 + 3) bludgeoning damage. If the target is a creature, it is grappled (escape DC 16). Until this grapple ends, the target is restrained, and the octopus can't use its tentacles on another target.
  - name: Ink Cloud (Recharges after a Short or Long Rest)
    text: A 20-foot-radius cloud of ink extends all around the octopus if it is underwater. The area is heavily obscured for 1 minute, although a significant current can disperse the ink. After releasing the ink, the octopus can use the Dash action as a bonus action.
---
