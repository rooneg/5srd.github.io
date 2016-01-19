---
title: Mummy Lord
size: Medium
type: undead
alignment: lawful evil
armor_class: 17
armor_class_descriptor: natural armor
hp: 97
hd: 13
speeds:
  - name: walk
    speed: 20
ability_scores:
  Strength: 18
  Dexterity: 10
  Constitution: 17
  Intelligence: 11
  Wisdom: 18
  Charisma: 16
saving_throw_proficiencies:
  - Constitution
  - Intelligence
  - Wisdom
  - Charisma
skills:
  - name: History
    bonus: 5
  - name: Religion
    bonus: 5
damage_vulnerabilities:
  - fire
damage_immunities:
  - necrotic
  - poison
  - bludgeoning, piercing, and slashing from nonmagical attacks
condition_immunities:
  - charmed
  - exhaustion
  - frightened
  - paralyzed
  - poisoned
senses:
  - name: darkvision
    range: 60
languages:
  - the languages it knew in life
challenge: 15
special_traits:
  - name: Magic Resistance
    text: The mummy lord has advantage on saving throws against spells and other magical effects.
  - name: Rejuvenation
    text: A destroyed mummy lord gains a new body in 24 hours if its heart is intact, regaining all its hit points and becoming active again. The new body appears within 5 feet of the mummy lord's heart.
  - name: Spellcasting
    text: |
      The mummy lord is a 10th-level spellcaster. Its spellcasting ability is Wisdom (spell save DC 17, +9 to hit with spell attacks). The mummy lord has the following cleric spells prepared:

      - Cantrips (at will): *sacred flame*, *thaumaturgy*
      - 1st level (4 slots): *command*, *guiding bolt*, *shield of faith*
      - 2nd level (3 slots): *hold person*, *silence*, *spiritual weapon*
      - 3rd level (3 slots): *animate dead*, *dispel magic*
      - 4th level (3 slots): *divination*, *guardian of faith*
      - 5th level (2 slots): *contagion*, *insect plague*
      - 6th level (1 slot): *harm*
actions:
  - name: Multiattack
    text: The mummy can use its Dreadful Glare and makes one attack with its rotting fist.
  - name: Rotting Fist
    text: |
      *Melee Weapon Attack:* +9 to hit, reach 5  ft., one target. *Hit:* 14 (3d6 + 4) bludgeoning damage plus 21 (6d6) necrotic damage. If the target is a creature, it must succeed on a DC 16 Constitution saving throw or be cursed with mummy rot. The cursed target can't regain hit points, and its hit point maximum decreases by 10 (3d6) for every 24 hours that elapse. If the curse reduces the target's hit point maximum to 0, the target dies, and its body turns to dust. The curse lasts until removed by the remove curse spell or other magic.
  - name: Dreadful Glare
    text: The mummy lord targets one creature it can see within 60 feet of it. If the target can see the mummy lord, it must succeed on a DC 16 Wisdom saving throw against this magic or become frightened until the end of the mummy's next turn. If the target fails the saving throw by 5 or more, it is also paralyzed for the same duration. A target that succeeds on the saving throw is immune to the Dreadful Glare of all mummies and mummy lords for the next 24 hours.
legendary_actions:
  - name: Attack
    text: The mummy lord makes one attack with its rotting fist or uses its Dreadful Glare.
  - name: Blinding Dust
    text: Blinding dust and sand swirls magically around the mummy lord. Each creature within 5 feet of the mummy lord must succeed on a DC 16 Constitution saving throw or be blinded until the end of the creature's next turn.
  - name: Blasphemous Word (Costs 2 Actions)
    text: The mummy lord utters a blasphemous word. Each non-undead creature within 10 feet of the mummy lord that can hear the magical utterance must succeed on a DC 16  Constitution saving throw or be stunned until the end of the mummy lord's next turn.
  - name: Channel Negative Energy (Costs 2 Actions)
    text: The mummy lord magically unleashes negative energy. Creatures within 60 feet of the mummy lord, including ones behind barriers and around corners, can't regain hit points until the end of the mummy lord's next turn.
  - name: Whirlwind of Sand (Costs 2 Actions)
    text: The mummy lord magically transforms into a whirlwind of sand, moves up to 60 feet, and reverts to its normal form. While in whirlwind form, the mummy lord is immune to all damage, and it can't be grappled, petrified, knocked prone, restrained, or stunned. Equipment worn or carried by the mummy lord remain in its possession.
---

> **Source:** *Pathfinder Roleplaying Game Bestiary 5*.
>
> Many cultures practice the sacred art of mummification, though the sinister magical techniques used to imbue corpses with undead vitality are far less widespread. In certain ancient lands, such blasphemous techniques have been refined through centuries of ceremony and countless deaths, giving rise to mummies of terrible power. On rare occasions, if the deceased was of great rank and exceeding malevolence, he might undergo such elaborate rituals, rising from his tomb as a fearful mummy lord. Similarly, a ruler known for his malice or who died in a moment of great rage might spontaneously arise as such a vengeful despot. Regardless of the exact circumstances of his resurrection, a mummy lord retains the abilities he had in life, becoming a creature consumed by the desire to restore his rule and dominate both the living and dead.
