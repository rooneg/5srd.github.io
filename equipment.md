---
title: Equipment
source: |
 [System Reference Document 5.0](https://dnd.wizards.com/articles/features/systems-reference-document-srd)
nav: true
layout: ogl-notice
---

Common coins come in several different denominations based on the relative worth of the metal from which they are made. The three most common coins are the gold piece (gp), the silver piece (sp), and the copper piece (cp).

With one gold piece, a character can buy a bedroll, 50 feet of good rope, or a goat. A skilled (but not exceptional) artisan can earn one gold piece a day. The gold piece is the standard unit of measure for wealth, even if the coin itself is not commonly used. When merchants discuss deals that involve goods or services worth hundreds or thousands of gold pieces, the transactions don't usually involve the exchange of individual coins. Rather, the gold piece is a standard measure of value, and the actual exchange is in gold bars, letters of credit, or valuable goods.

One gold piece is worth ten silver pieces, the most prevalent coin among commoners. A silver piece buys a laborer's work for half a day, a flask of lamp oil, or a night's rest in a poor inn.

One silver piece is worth ten copper pieces, which are common among laborers and beggars. A single copper piece buys a candle, a torch, or a piece of chalk.

In addition, unusual coins made of other precious metals sometimes appear in treasure hoards. The electrum piece (ep) and the platinum piece (pp) originate from fallen empires and lost kingdoms, and they sometimes arouse suspicion and skepticism when used in transactions. An electrum piece is worth five silver pieces, and a platinum piece is worth ten gold pieces.

A standard coin weighs about a third of an ounce, so fifty coins weigh a pound.

| Coin          |    CP |   SP |   EP |    GP |     PP |
|:--------------|------:|-----:|-----:|------:|-------:|
| Copper (cp)   |     1 | 1/10 | 1/50 | 1/100 | 1/1000 |
| Silver (sp)   |    10 |    1 |  1/5 |  1/10 |  1/100 |
| Electrum (ep) |    50 |    5 |    1 |   1/2 |   1/20 |
| Gold (gp)     |   100 |   10 |    2 |     1 |   1/10 |
| Platinum (pp) | 1,000 |  100 |   20 |    10 |      1 |

## Selling Treasure

Opportunities abound to find treasure, equipment, weapons, armor, and more in the dungeons you explore. Normally, you can sell your treasures and trinkets when you return to a town or other settlement, provided that you can find buyers and merchants interested in your loot.

**Arms, Armor, and Other Equipment.** As a general rule, undamaged weapons, armor, and other equipment fetch half their cost when sold in a market. Weapons and armor used by monsters are rarely in good enough condition to sell.

**Magic Items.** Selling magic items is problematic. Finding someone to buy a potion or a scroll isn't too hard, but other items are out of the realm of most but the wealthiest nobles. Likewise, aside from a few common magic items, you won't normally come across magic items or spells to purchase. The value of magic is far beyond simple gold and should always be treated as such.

**Gems, Jewelry, and Art Objects.** These items retain their full value in the marketplace, and you can either trade them in for coin or use them as currency for other transactions. For exceptionally valuable treasures, the GM might require you to find a buyer in a large town or larger community first.

**Trade Goods.** On the borderlands, many people conduct transactions through barter. Like gems and art objects, trade goods---bars of iron, bags of salt, livestock, and so on---retain their full value in the market and can be used as currency.

### Armor

Fantasy gaming worlds are a vast tapestry made up of many different cultures, each with its own technology level. For this reason, adventurers have access to a variety of armor types, ranging from leather armor to chain mail to costly plate armor, with several other kinds of armor in between. The Armor table collects the most commonly available types of armor found in the game and separates them into three categories: light armor, medium armor, and heavy armor. Many warriors supplement their armor with a shield.

The table shows the cost, weight, and other properties of the common types of armor worn in fantasy gaming worlds.

**Armor Proficiency.** Anyone can put on a suit of armor or strap a shield to an arm. Only those proficient in the armor's use know how to wear it effectively, however. Your class gives you proficiency with certain types of armor. If you wear armor that you lack proficiency with, you have disadvantage on any ability check, saving throw, or attack roll that involves Strength or Dexterity, and you can't cast spells.

**Armor Class (AC).** Armor protects its wearer from attacks. The armor (and shield) you wear determines your base Armor Class.

**Light Armor.** Made from supple and thin materials, light armor favors agile adventurers since it offers some protection without sacrificing mobility. If you wear light armor, you add your Dexterity modifier to the base number from your armor type to determine your Armor Class.

**Medium Armor.** Medium armor offers more protection than light armor, but it also impairs movement more. If you wear medium armor, you add your Dexterity modifier, to a maximum of +2, to the base number from your armor type to determine your Armor Class.

**Heavy Armor.** Of all the armor categories, heavy armor offers the best protection. These suits of armor cover the entire body and are designed to stop a wide range of attacks. Only proficient warriors can manage their weight and bulk. If the Armor table shows "Str 13" or "Str 15" in the Strength column for an armor type, the armor reduces the wearer's speed by 10 feet unless the wearer has a Strength score equal to or higher than the listed score. Heavy armor doesn't let you add your Dexterity modifier to your Armor Class, but it also doesn't penalize you if your Dexterity modifier is negative.

**Stealth.** If the Armor table shows "Disadvantage" in the Stealth column, the wearer has disadvantage on Dexterity (Stealth) checks.

{% assign armor_groups = site.equipment | where: 'category', 'Armor' | group_by: 'subcategory' %}
{% for armor_group in armor_groups %}
  {% assign armors_sorted = armor_group.items | sort: 'title' %}
  <table class="fullwidth">
    <thead>
      <tr>
        <th>{{ armor_group.name }} {% if armor_group.name != 'Shield' %}armors{% endif %}</th>
        <th>Armor class</th>
        <th style="text-align: right;">Strength</th>
        <th>Stealth</th>
        <th style="text-align: right;">Cost</th>
        <th style="text-align: right;">Weight</th>
      </tr>
    </thead>
    <tbody>
      {% for armor in armors_sorted %}
        <tr>
          <td><a href="{{ armor.url }}">{{ armor.title }}</a></td>
          <td>
            {% if armor.subcategory == 'Shield' %}+{% endif %}{{ armor.armor_class }}
            {% if armor.subcategory == 'Light' or armor.subcategory == 'Medium' %}
              + Dex {% if armor.subcategory == 'Medium' %}(max 2){% endif %}
            {% endif %}
          </td>
          <td style="text-align: right;">{% if armor.strength_requirement == '---' %}&mdash;{% else %}{{ armor.strength_requirement }}{% endif %}</td>
          <td>{% if armor.stealth_disadvantage %}Disadvantage{% else %}&mdash;{% endif %}</td>
          <td style="text-align: right;">{% include format_cost.html cost=armor.cost %}</td>
          <td style="text-align: right;">{% include format_weight.html weight=armor.weight %}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
{% endfor %}

#### Getting Into and Out of Armor

The time it takes to don or doff armor depends on the armor's category.

**Don.** This is the time it takes to put on armor. You benefit from the armor's AC only if you take the full time to don the suit of armor.

**Doff.** This is the time it takes to take off armor. If you have help, reduce this time by half.

| Category     |    Don     |   Doff    |
|:-------------|:----------:|:---------:|
| light armor  |  1 minute  | 1 minute  |
| medium armor | 5 minutes  | 1 minute  |
| heavy armor  | 10 minutes | 5 minutes |
| shield       |  1 action  | 1 action  |

## Weapons

Your class grants proficiency in certain weapons, reflecting both the class's focus and the tools you are most likely to use. Whether you favor a longsword or a longbow, your weapon and your ability to wield it effectively can mean the difference between life and death while adventuring.

The table shows the most common weapons used in the fantasy gaming worlds, their price and weight, the damage they deal when they hit, and any special properties they possess. Every weapon is classified as either melee or ranged. A melee weapon is used to attack a target within 5 feet of you, whereas a ranged weapon is used to attack a target at a distance.

{% assign weapon_groups = site.equipment | where: 'category', 'Weapon' | group_by: 'subcategory' %}
{% for weapon_group in weapon_groups %}
  {% assign weapons_sorted = weapon_group.items | sort: 'title' %}
  <table class="fullwidth">
    <thead>
      <tr>
        <th>{{ weapon_group.name }} weapons</th>
        <th style="text-align: left;">Damage</th>
        <th style="text-align: left;">Properties</th>
        <th style="text-align: right;">Cost</th>
        <th style="text-align: right;">Weight</th>
      </tr>
    </thead>
    <tbody>
      {% for weapon in weapons_sorted %}
        <tr>
          <td><a href="{{ weapon.url }}">{{ weapon.title }}</a></td>
          <td>{{ weapon.damage }} {{ weapon.damage_type }}</td>
          <td>{% if weapon.properties %}{{ weapon.properties | array_to_sentence_string }}{% else %}&mdash;{% endif %}</td>
          <td style="text-align: right;">{% include format_cost.html cost=weapon.cost %}</td>
          <td style="text-align: right;">{% include format_weight.html weight=weapon.weight %}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
{% endfor %}

### Weapon Proficiency

Your race, class, and feats can grant you proficiency with certain weapons or categories of weapons. The two categories are simple and martial. Most people can use simple weapons with proficiency. These weapons include clubs, maces, and other weapons often found in the hands of commoners. Martial weapons, including swords, axes, and polearms, require more specialized training to use effectively. Most warriors use martial weapons because these weapons put their fighting style and training to best use.

Proficiency with a weapon allows you to add your proficiency bonus to the attack roll for any attack you make with that weapon. If you make an attack roll using a weapon with which you lack proficiency, you do not add your proficiency bonus to the attack roll.

### Weapon Properties

Many weapons have special properties related to their use, as shown in the table.

**Ammunition.** You can use a weapon that has the ammunition property to make a ranged attack only if you have ammunition to fire from the weapon. Each time you attack with the weapon, you expend one piece of ammunition. Drawing the ammunition from a quiver, case, or other container is part of the attack (you need a free hand to load a one-handed weapon). At the end of the battle, you can recover half your expended ammunition by taking a minute to search the battlefield.

If you use a weapon that has the ammunition property to make a melee attack, you treat the weapon as an improvised weapon (see "Improvised Weapons"). A sling must be loaded to deal any damage when used in this way.

**Finesse.** When making an attack with a finesse weapon, you use your choice of your Strength or Dexterity modifier for the attack and damage rolls. You must use the same modifier for both rolls.

**Heavy.** Small creatures have disadvantage on attack rolls with heavy weapons. A heavy weapon's size and bulk make it too large for a Small creature to use effectively.

**Light.** A light weapon is small and easy to handle, making it ideal for use when fighting with two weapons.

**Loading.** Because of the time required to load this weapon, you can fire only one piece of ammunition from it when you use an action, bonus action, or reaction to fire it, regardless of the number of attacks you can normally make.

**Range.** A weapon that can be used to make a ranged attack has a range in parentheses after the ammunition or thrown property. The range lists two numbers. The first is the weapon's normal range in feet, and the second indicates the weapon's long range. When attacking a target beyond normal range, you have disadvantage on the attack roll. You can't attack a target beyond the weapon's long range.

**Reach.** This weapon adds 5 feet to your reach when you attack with it, as well as when determining your reach for opportunity attacks with it.

**Special.** A weapon with the special property has unusual rules governing its use, explained in the weapon's description (see "Special Weapons" later in this section).

**Thrown.** If a weapon has the thrown property, you can throw the weapon to make a ranged attack. If the weapon is a melee weapon, you use the same ability modifier for that attack roll and damage roll that you would use for a melee attack with the weapon. For example, if you throw a handaxe, you use your Strength, but if you throw a dagger, you can use either your Strength or your Dexterity, since the dagger has the finesse property.

**Two-Handed.** This weapon requires two hands when you attack with it.

**Versatile.** This weapon can be used with one or two hands. A damage value in parentheses appears with the property---the damage when the weapon is used with two hands to make a melee attack.

### Improvised Weapons

Sometimes characters don't have their weapons and have to attack with whatever is at hand. An improvised weapon includes any object you can wield in one or two hands, such as broken glass, a table leg, a frying pan, a wagon wheel, or a dead goblin.

Often, an improvised weapon is similar to an actual weapon and can be treated as such. For example, a table leg is akin to a club. At the GM's option, a character proficient with a weapon can use a similar object as if it were that weapon and use his or her proficiency bonus.

An object that bears no resemblance to a weapon deals 1d4 damage (the GM assigns a damage type appropriate to the object). If a character uses a ranged weapon to make a melee attack, or throws a melee weapon that does not have the thrown property, it also deals 1d4 damage. An improvised thrown weapon has a normal range of 20 feet and a long range of 60 feet.

### Silvered Weapons

Some monsters that have immunity or resistance to nonmagical weapons are susceptible to silver weapons, so cautious adventurers invest extra coin to plate their weapons with silver. You can silver a single weapon or ten pieces of ammunition for 100 gp. This cost represents not only the price of the silver, but the time and expertise needed to add silver to the weapon without making it less effective.

## Adventuring Gear

{% assign gears = site.equipment | where: 'category', 'Gear' | sort_by: 'title' %}
<table>
  <thead>
    <tr>
      <th>Gear</th>
      <th style="text-align: right;">Cost</th>
      <th style="text-align: right;">Weight</th>
    </tr>
  </thead>
  <tbody>
    {% for gear in gears %}
    <tr>
      <td><a href="{{ gear.url }}">{{ gear.title }}</a></td>
      <td style="text-align: right;">{% include format_cost.html cost=gear.cost %}</td>
      <td style="text-align: right;">{% include format_weight.html weight=gear.weight %}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

### Equipment Packs

The starting equipment you get from your class includes a collection of useful adventuring gear, put together in a pack. The contents of these packs are listed here. If you are buying your starting equipment, you can purchase a pack for the price shown, which might be cheaper than buying the items individually.

{% assign packs = site.equipment | where: 'category', 'Pack' | sort_by: 'title' %}
<table>
  <thead>
    <tr>
      <th>Equipment packs</th>
      <th style="text-align: right;">Cost</th>
      <th style="text-align: right;">Weight</th>
    </tr>
  </thead>
  <tbody>
    {% for pack in packs %}
    <tr>
      <td><a href="{{ pack.url }}">{{ pack.title }}</a></td>
      <td style="text-align: right;">{% include format_cost.html cost=pack.cost %}</td>
      <td style="text-align: right;">{% include format_weight.html weight=pack.weight %}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

## Tools

A tool helps you to do something you couldn't otherwise do, such as craft or repair an item, forge a document, or pick a lock. Your race, class, background, or feats give you proficiency with certain tools. Proficiency with a tool allows you to add your proficiency bonus to any ability check you make using that tool. Tool use is not tied to a single ability, since proficiency with a tool represents broader knowledge of its use. For example, the GM might ask you to make a Dexterity check to carve a fine detail with your woodcarver's tools, or a Strength check to make something out of particularly hard wood.

{% assign tools = site.equipment | where: 'category', 'Tool' | sort_by: 'title' %}
<table>
  <thead>
    <tr>
      <th>Tools</th>
      <th style="text-align: right;">Cost</th>
      <th style="text-align: right;">Weight</th>
    </tr>
  </thead>
  <tbody>
    {% for tool in tools %}
    <tr>
      <td><a href="{{ tool.url }}">{{ tool.title }}</a></td>
      <td style="text-align: right;">{% include format_cost.html cost=tool.cost %}</td>
      <td style="text-align: right;">{% include format_weight.html weight=tool.weight %}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>

## Mounts and Vehicles

A good mount can help you move more quickly through the wilderness, but its primary purpose is to carry the gear that would otherwise slow you down. The Mounts and Other Animals table shows each animal's speed and base carrying capacity.

An animal pulling a carriage, cart, chariot, sled, or wagon can move weight up to five times its base carrying capacity, including the weight of the vehicle. If multiple animals pull the same vehicle, they can add their carrying capacity together.

Mounts other than those listed here are available in fantasy gaming worlds, but they are rare and not normally available for purchase. These include flying mounts (pegasi, griffons, hippogriffs, and similar animals) and even aquatic mounts (giant sea horses, for example). Acquiring such a mount often means securing an egg and raising the creature yourself, making a bargain with a powerful entity, or negotiating with the mount itself.

| Mount                                    |   Cost |  Speed |  Capacity |
|:-----------------------------------------|-------:|-------:|----------:|
| [camel](/monsters/camel/)                |  50 gp | 50 ft. |   480 lb. |
| [donkey or mule](/monsters/mule/)        |   8 gp | 40 ft. |   420 lb. |
| [elephant](/monsters/elephant/)          | 200 gp | 40 ft. | 1,320 lb. |
| [horse, draft](/monsters/horse-draft/)   |  50 gp | 40 ft. |   540 lb. |
| [horse, riding](/monsters/horse-riding/) |  75 gp | 60 ft. |   480 lb. |
| [mastiff](/monsters/mastiff/)            |  25 gp | 40 ft. |   195 lb. |
| [pony](/monsters/horse-pony/)            |  30 gp | 40 ft. |   225 lb. |
| [warhorse](/monsters/horse-warhorse/)    | 400 gp | 60 ft. |   540 lb. |

| Tack and harness   |   Cost |  Weight |
|:-------------------|-------:|--------:|
| barding            |     ×4 |      ×2 |
| bit and bridle     |   2 gp |   1 lb. |
| carriage           | 100 gp | 600 lb. |
| cart               |  15 gp | 200 lb. |
| chariot            | 250 gp | 100 lb. |
| feed (per day)     |   5 cp |  10 lb. |
| saddle, exotic     |  60 gp |  40 lb. |
| saddle, military   |  20 gp |  30 lb. |
| saddle, pack       |   5 gp |  15 lb. |
| saddle, riding     |  10 gp |  25 lb. |
| saddlebags         |   4 gp |   8 lb. |
| sled               |  20 gp | 300 lb. |
| stabling (per day) |   5 sp |     --- |
| wagon              |  35 gp | 400 lb. |

| Water vehicle |      Cost |     Speed |
|:--------------|----------:|----------:|
| keelboat      |  3,000 gp |     1 mph |
| rowboat       |     50 gp | 1-1⁄2 mph |
| warship       | 25,000 gp | 2-1⁄2 mph |
| galley        | 30,000 gp |     4 mph |
| longship      | 10,000 gp |     3 mph |
| sailing ship  | 10,000 gp |     2 mph |

**Barding.** Barding is armor designed to protect an animal's head, neck, chest, and body. Any type of armor shown on the Armor table can be purchased as barding. The cost is four times the equivalent armor made for humanoids, and it weighs twice as much.

**Saddles.** A military saddle braces the rider, helping you keep your seat on an active mount in battle. It gives you advantage on any check you make to remain mounted. An exotic saddle is required for riding any aquatic or flying mount.

**Vehicle Proficiency.** If you have proficiency with a certain kind of vehicle (land or water), you can add your proficiency bonus to any check you make to control that kind of vehicle in difficult circumstances.

**Rowed Vessels.** Keelboats and rowboats are used on lakes and rivers. If going downstream, add the speed of the current (typically 3 miles per hour) to the speed of the vehicle. These vehicles can't be rowed against any significant current, but they can be pulled upstream by draft animals on the shores. A rowboat weighs 100 pounds, in case adventurers carry it over land.

## Trade Goods

Most wealth is not in coins. It is measured in livestock, grain, land, rights to collect taxes, or rights to resources (such as a mine or a forest).

Guilds, nobles, and royalty regulate trade. Chartered companies are granted rights to conduct trade along certain routes, to send merchant ships to various ports, or to buy or sell specific goods. Guilds set prices for the goods or services that they control, and determine who may or may not offer those goods and services. Merchants commonly exchange trade goods without using currency. The Trade Goods table shows the value of commonly exchanged goods.

|   Cost | Goods                                        |
|-------:|:---------------------------------------------|
|   1 cp | 1 lb. of wheat                               |
|   2 cp | 1 lb. of flour or one chicken                |
|   5 cp | 1 lb. of salt                                |
|   1 sp | 1 lb. of iron or 1 sq. yd. of canvas         |
|   5 sp | 1 lb. of copper or 1 sq. yd. of cotton cloth |
|   1 gp | 1 lb. of ginger or one goat                  |
|   2 gp | 1 lb. of cinnamon or pepper, or one sheep    |
|   3 gp | 1 lb. of cloves or one pig                   |
|   5 gp | 1 lb. of silver or 1 sq. yd. of linen        |
|  10 gp | 1 sq. yd. of silk or one cow                 |
|  15 gp | 1 lb. of saffron or one ox                   |
|  50 gp | 1 lb. of gold                                |
| 500 gp | 1 lb. of platinum                            |

## Expenses

When not descending into the depths of the earth, exploring ruins for lost treasures, or waging war against the encroaching darkness, adventurers face more mundane realities. Even in a fantastical world, people require basic necessities such as shelter, sustenance, and clothing. These things cost money, although some lifestyles cost more than others.

### Lifestyle Expenses

Lifestyle expenses provide you with a simple way to account for the cost of living in a fantasy world. They cover your accommodations, food and drink, and all your other necessities. Furthermore, expenses cover the cost of maintaining your equipment so you can be ready when adventure next calls.

At the start of each week or month (your choice), choose a lifestyle from the Expenses table and pay the price to sustain that lifestyle. The prices listed are per day, so if you wish to calculate the cost of your chosen lifestyle over a thirty-day period, multiply the listed price by 30. Your lifestyle might change from one period to the next, based on the funds you have at your disposal, or you might maintain the same lifestyle throughout your character's career.

Your lifestyle choice can have consequences. Maintaining a wealthy lifestyle might help you make contacts with the rich and powerful, though you run the risk of attracting thieves. Likewise, living frugally might help you avoid criminals, but you are unlikely to make powerful connections.

| Lifestyle    |     Price/Day |
|:-------------|--------------:|
| wretched     |           --- |
| squalid      |          1 sp |
| poor         |          2 sp |
| modest       |          1 gp |
| comfortable  |          2 gp |
| wealthy      |          4 gp |
| aristocratic | 10 gp minimum |

**Wretched.** You live in inhumane conditions. With no place to call home, you shelter wherever you can, sneaking into barns, huddling in old crates, and relying on the good graces of people better off than you. A wretched lifestyle presents abundant dangers. Violence, disease, and hunger follow you wherever you go. Other wretched people covet your armor, weapons, and adventuring gear, which represent a fortune by their standards. You are beneath the notice of most people.

**Squalid.** You live in a leaky stable, a mud-floored hut just outside town, or a vermin-infested boarding house in the worst part of town. You have shelter from the elements, but you live in a desperate and often violent environment, in places rife with disease, hunger, and misfortune. You are beneath the notice of most people, and you have few legal protections. Most people at this lifestyle level have suffered some terrible setback. They might be disturbed, marked as exiles, or suffer from disease.

**Poor.** A poor lifestyle means going without the comforts available in a stable community. Simple food and lodgings, threadbare clothing, and unpredictable conditions result in a sufficient, though probably unpleasant, experience. Your accommodations might be a room in a flophouse or in the common room above a tavern. You benefit from some legal protections, but you still have to contend with violence, crime, and disease. People at this lifestyle level tend to be unskilled laborers, costermongers, peddlers, thieves, mercenaries, and other disreputable types.

**Modest.** A modest lifestyle keeps you out of the slums and ensures that you can maintain your equipment. You live in an older part of town, renting a room in a boarding house, inn, or temple. You don't go hungry or thirsty, and your living conditions are clean, if simple. Ordinary people living modest lifestyles include soldiers with families, laborers, students, priests, hedge wizards, and the like.

**Comfortable.** Choosing a comfortable lifestyle means that you can afford nicer clothing and can easily maintain your equipment. You live in a small cottage in a middle-class neighborhood or in a private room at a fine inn. You associate with merchants, skilled tradespeople, and military officers.

**Wealthy.** Choosing a wealthy lifestyle means living a life of luxury, though you might not have achieved the social status associated with the old money of nobility or royalty. You live a lifestyle comparable to that of a highly successful merchant, a favored servant of the royalty, or the owner of a few small businesses. You have respectable lodgings, usually a spacious home in a good part of town or a comfortable suite at a fine inn. You likely have a small staff of servants.

**Aristocratic.** You live a life of plenty and comfort. You move in circles populated by the most powerful people in the community. You have excellent lodgings, perhaps a townhouse in the nicest part of town or rooms in the finest inn. You dine at the best restaurants, retain the most skilled and fashionable tailor, and have servants attending to your every need. You receive invitations to the social gatherings of the rich and powerful, and spend evenings in the company of politicians, guild leaders, high priests, and nobility. You must also contend with the highest levels of deceit and treachery. The wealthier you are, the greater the chance you will be drawn into political intrigue as a pawn or participant.

#### Self-Sufficiency

The expenses and lifestyles described here assume that you are spending your time between adventures in town, availing yourself of whatever services you can afford---paying for food and shelter, paying townspeople to sharpen your sword and repair your armor, and so on. Some characters, though,
might prefer to spend their time away from civilization, sustaining themselves in the wild by hunting, foraging, and repairing their own gear.

Maintaining this kind of lifestyle doesn't require you to spend any coin, but it is time-consuming. If you spend your time between adventures practicing a profession, you can eke out the equivalent of a poor lifestyle. Proficiency in the Survival skill lets you live at the equivalent of a comfortable lifestyle.

### Food, Drink, and Lodging

The Food, Drink, and Lodging table gives prices for individual food items and a single night's lodging. These prices are included in your total lifestyle expenses.

| Item                             |  Cost |
|:---------------------------------|------:|
| ale, gallon                      |  2 sp |
| ale, mug                         |  4 cp |
| banquet (per person)             | 10 gp |
| bread, loaf                      |  2 cp |
| cheese, hunk                     |  1 sp |
| inn stay, squalid (per day)      |  7 cp |
| inn stay, poor (per day)         |  1 sp |
| inn stay, modest (per day)       |  5 sp |
| inn stay, comfortable (per day)  |  8 sp |
| inn stay, wealthy (per day)      |  2 gp |
| inn stay, aristocratic (per day) |  4 gp |
| meals, squalid (per day)         |  3 cp |
| meals, poor (per day)            |  6 cp |
| meals, modest (per day)          |  3 sp |
| meals, comfortable (per day)     |  5 sp |
| meals, wealthy (per day)         |  8 sp |
| meals, aristocratic (per day)    |  2 gp |
| meat, chunk                      |  3 sp |
| wine, common (pitcher)           |  2 sp |
| wine, fine (bottle)              | 10 gp |

### Services

Adventurers can pay nonplayer characters to assist them or act on their behalf in a variety of circumstances. Most such hirelings have fairly ordinary skills, while others are masters of a craft or art, and a few are experts with specialized adventuring skills.

Some of the most basic types of hirelings appear on the table. Other common hirelings include any of the wide variety of people who inhabit a typical town or city, when the adventurers pay them to perform a specific task. For example, a wizard might pay a carpenter to construct an elaborate chest (and its miniature replica) for use in the secret chest spell. A fighter might commission a blacksmith to forge a special sword. A bard might pay a tailor to make exquisite clothing for an upcoming performance in front of the duke.

Other hirelings provide more expert or dangerous services. Mercenary soldiers paid to help the adventurers take on a hobgoblin army are hirelings, as are sages hired to research ancient or esoteric lore. If a high-level adventurer establishes a stronghold of some kind, he or she might hire a whole staff of servants and agents to run the place, from a castellan or steward to menial laborers to keep the stables clean. These hirelings often enjoy a long-term contract that includes a place to live within the stronghold as part of the offered compensation.

| Service                  | Pay           |
|:-------------------------|:--------------|
| coach cab, between towns | 3 cp per mile |
| coach cab, within a city | 1 cp          |
| hireling, skilled        | 2 gp per day  |
| hireling, untrained      | 2 sp per day  |
| messenger                | 2 cp per mile |
| road or gate toll        | 1 cp          |
| ship's passage           | 1 sp per mile |

Skilled hirelings include anyone hired to perform a service that involves a proficiency (including weapon, tool, or skill): a mercenary, artisan, scribe, and so on. The pay shown is a minimum; some expert hirelings require more pay. Untrained hirelings are hired for menial work that requires no particular skill and can include laborers, porters, maids, and similar workers.

### Spellcasting Services

People who are able to cast spells don't fall into the category of ordinary hirelings. It might be possible to find someone willing to cast a spell in exchange for coin or favors, but it is rarely easy and no established pay rates exist. As a rule, the higher the level of the desired spell, the harder it is to find someone who can cast it and the more it costs.

Hiring someone to cast a relatively common spell of 1st or 2nd level, such as [*cure wounds*](/spells/cure-wounds/) or [*identify*](/spells/identify/), is easy enough in a city or town, and might cost 10 to 50 gold pieces (plus the cost of any expensive material components). Finding someone able and willing to cast a higher-level spell might involve traveling to a large city, perhaps one with a university or prominent temple. Once found, the spellcaster might ask for a service instead of payment---the kind of service that only adventurers can provide, such as retrieving a rare item from a dangerous locale or traversing a monster-infested wilderness to deliver something important to a distant settlement.
