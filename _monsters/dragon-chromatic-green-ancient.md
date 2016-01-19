---
title: Dragon, Chromatic, Green, Ancient
size: Gargantuan
type: dragon
alignment: lawful evil
armor_class: 21
armor_class_descriptor: natural armor
hp: 385
hd: 22
speeds:
  - name: walk
    speed: 40
  - name: fly
    speed: 80
  - name: swim
    speed: 40
ability_scores:
  Strength: 27
  Dexterity: 12
  Constitution: 25
  Intelligence: 20
  Wisdom: 17
  Charisma: 19
saving_throw_proficiencies:
  - Dexterity
  - Constitution
  - Wisdom
  - Charisma
skills:
  - name: Deception
    bonus: 11
  - name: Insight
    bonus: 10
  - name: Perception
    bonus: 17
  - name: Persuasion
    bonus: 11
  - name: Stealth
    bonus: 8
damage_immunities:
  - poison
condition_immunities:
  - poisoned
senses:
  - name: blindsight
    range: 60
  - name: darkvision
    range: 120
languages:
  - Common
  - Draconic
challenge: 22
special_traits:
  - name: Amphibious
    text: The dragon can breathe air and water.
  - name: Legendary Resistance (3/Day)
    text: If the dragon fails a saving throw, it can choose to succeed instead.
actions:
  - name: Multiattack
    text: |
       The dragon can use its Frightful Presence. It then makes three attacks: one with its bite and two with its claws.
  - name: Bite
    text: |
       *Melee Weapon Attack:* +15 to hit, reach 15 ft., one target. *Hit:* 19 (2d10 + 8) piercing damage plus 10 (3d6) poison damage.
  - name: Claw
    text: |
       *Melee Weapon Attack:* +15 to hit, reach 10 ft., one target. *Hit:* 22 (4d6 + 8) slashing damage.
  - name: Tail
    text: |
      *Melee Weapon Attack:* +15 to hit, reach 20 ft., one target. *Hit:* 17 (2d8 + 8) bludgeoning damage.
  - name: Frightful Presence
    text: Each creature of the dragon's choice that is within 120 feet of the dragon and aware of it must succeed on a DC 19 Wisdom saving throw or become frightened for 1 minute. A creature can repeat the saving throw at the end of each of its turns, ending the effect on itself on a success. If a creature's saving throw is successful or the effect ends for it, the creature is immune to the dragon's Frightful Presence for the next 24 hours.
  - name: Poison Breath (Recharge 5--6)
    text: The dragon exhales poisonous gas in a 90-foot cone. Each creature in that area must make a DC 22 Constitution saving throw, taking 77 (22d6) poison damage on a failed save, or half as much damage on a successful one.
legendary_actions:
  - name: Detect
    text: The dragon makes a Wisdom (Perception) check.
  - name: Tail Attack
    text: The dragon makes a tail attack.
  - name: Wing Attack (Costs 2 Actions)
    text: The dragon beats its wings. Each creature within 15 feet of the dragon must succeed on a DC 23 Dexterity saving throw or take 15 (2d6 + 8) bludgeoning damage and be knocked prone. The dragon can then fly up to half its flying speed.
---

> **Source:** *Pathfinder Roleplaying Game Bestiary*.
>
> Green dragons dwell in the ancient forests of the world, prowling under towering canopies in search of prey. Of all the chromatic dragons, green dragons are perhaps the easiest to deal with diplomatically.
