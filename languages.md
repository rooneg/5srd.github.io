---
title: Languages
nav: true
---

<div class="col-md-6 pull-md-right">
  {% assign language_groups = site.languages | group_by: 'group' %}
  {% for language_group in language_groups %}
  <table class="table table-sm">
    <caption>{{ language_group.name | capitalize }} Languages</caption>
    <thead>
      <tr>
        <th>Language</th>
        <th>Typical Speakers</th>
        <th>Script</th>
      </tr>
    </thead>
    <tbody>
    {% for language in language_group.items %}
      <tr>
        <td><a href="{{ language.url }}">{{ language.title }}</a></td>
        <td>{{ language.typical_speakers | array_to_sentence_string }}</td>
        <td>{{ language.script }}</td>
    {% endfor %}
    </tbody>
  </table>
  {% endfor %}
</div>

Your race indicates the languages your character can speak by default, and your background might give you access to one or more additional languages of your choice. Note these languages on your character sheet.

Choose your languages from the Standard Languages table, or choose one that is common in your campaign. With your GM’s permission, you can instead choose a language from the Exotic Languages table or a secret language, such as thieves’ cant or the tongue of druids.

Some of these languages are actually families of languages with many dialects. For example, the [Primordial](/languages/primordial/) language includes the Auran, Aquan, Ignan, and Terran dialects, one for each of the four elemental planes. Creatures that speak different dialects of the same language can communicate with one another.
