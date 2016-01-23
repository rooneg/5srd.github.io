---
title: Clay Golem
source: |
  [System Reference Document 5.0](https://dnd.wizards.com/articles/features/systems-reference-document-srd)
size: Large
type: construct
alignment: unaligned
armor_class: 14
armor_class_descriptor: natural armor
hp: 133
hd: 14
speeds:
  - name: walk
    speed: 20
ability_scores:
  Strength: 20
  Dexterity: 9
  Constitution: 18
  Intelligence: 3
  Wisdom: 8
  Charisma: 1
damage_immunities:
  - acid, poison, psychic; bludgeoning, piercing, and slashing from nonmagical attacks that aren't adamantine
condition_immunities:
  - charmed
  - exhaustion
  - frightened
  - paralyzed
  - petrified
  - poisoned
senses:
  - name: darkvision
    range: 60
languages:
  - understands the languages of its creator but can't speak
challenge: 9
special_traits:
  - name: Acid Absorption
    text: Whenever the golem is subjected to acid damage, it takes no damage and instead regains a number of hit points equal to the acid damage dealt.
  - name: Berserk
    text: Whenever the golem starts its turn with 60 hit points or fewer, roll a d6. On a 6, the golem goes berserk. On each of its turns while berserk, the golem attacks the nearest creature it can see. If no creature is near enough to move to and attack, the golem attacks an object, with preference for an object smaller than itself. Once the golem goes berserk, it continues to do so until it is destroyed or regains all its hit points.
  - name: Immutable Form
    text: The golem is immune to any spell or effect that would alter its form.
  - name: Magic Resistance
    text: The golem has advantage on saving throws against spells and other magical effects.
  - name: Magic Weapons
    text: The golem's weapon attacks are magical.
actions:
  - name: Multiattack
    text: The golem makes two slam attacks.
  - name: Slam
    text: |
      *Melee Weapon Attack:* +8 to hit, reach 5 ft., one target. *Hit:* 16 (2d10 + 5) bludgeoning damage. If the target is a creature, it must succeed on a DC 15  Constitution saving throw or have its hit point maximum reduced by an amount equal to the damage taken. The target dies if this attack reduces its hit point maximum to 0. The reduction lasts until removed by the greater restoration spell or other magic.
  - name: Haste (Recharge 5--6)
    text: Until the end of its next turn, the golem magically gains a +2 bonus to its AC, has advantage on Dexterity saving throws, and can use its slam attack as a bonus action.
---

> **Source:** *Pathfinder Roleplaying Game Bestiary*.
>
> A clay golem wears no clothing except for a metal or stiff leather garment around its hips. It stands over 8 feet tall and weighs 600 pounds.
