## Vereisten

Om een nieuwsbericht te maken heb je minstens 2 dingen nodig

- Een tekst
- Een foto (om je nieuwsbericht aantrekkelijker te maken wanneer het op social media gedeeld wordt)

Lees ook eerst het document over hoe je [een voorstel moet maken](/processes/voorstellen-indienen.md) of hoe je [wijzigingen doorvoert aan een bestaand voorstel](/processes/voorstellen-wijzigen.md).

## Maak een pull request aan voor de tekst

Ga naar de `Code` tab in de repository en navigeer naar `_content\news\_posts\` en klik op de `Create new file` knop.

In het bovenste tekst vak geef je het bestand een naam in de vorm `yyyy-mm-dd-je-titel.markdown`.

In het `Edit new file` vak dien je de inhoud van het bestand te voorzien, deze inhoud bestaat uit 2 delen
* Frontmatter: de metadata over het nieuwsbericht, in YAML formaat
* Body: het nieuwsbericht zelf, in Markdown formaat

Hieronder worden beide secties toegelicht, maar om het makkelijker te maken is er een [template voorzien](/templates/assets/newsitem.md) die je kan copy pasten.

### Frontmatter

Het eerste stuk van het document wordt de Frontmatter genoemd. Het beschrijft de inhoud van het document aan de website render engine, zodat die alerlei zaken kan automatiseren.

De frontmatter, staat tussen 2 regels met elk 3 koppeltekens: `---`, en moet minstens volgende velden bevatten (LET OP: geen hoofdletters gebruiken in de veldnamen!)

* layout: Dit veld beschrijft hoe de pagina gerendered moet worden, in geval van een nieuwsitem is dit altijd de waarde `post`.
* title:  Dit is de titel van het bericht, die wordt gebruikt in het overzicht, bovenaan het nieuwsbericht en op social media integratie.
* cover: Dit is een link naar de foto die als cover gebruikt dient te worden wanneer het bericht gedeeld wordt op social media, de link volgt het formaat `/news/img/uwfoto.png`
* date: Dit is de datum van het bericht, is enkel relevant binnen de sortering in het nieuwsoverzicht, het formaat is yyy-mm-dd HH:MM:ss
* description: Vul hier een beschrijving in, deze wordt gebruikt in het overzicht en ook wanneer de link op social media wordt gedeeld.
* permalink: Dit is link naar de pagina, die in het overzicht gebruikt wordt. Het formaat is `/news/vervang-dit-door-de-bestandsnaam-zonder-extensie/`

### Body

Hier plak je de tekst van je bericht zonder opmaak. De opmaak dien je te voorzien aan de hand van de markdown notatie. De [template](/templates/assets/newsitem.md) beschrijft de meest courante elementen al. Voor meer gedetailleerde info voer de markdown notatie kan je terecht op [deze handige cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Commit new file

Verzorg een *betekenisvolle titel* en *beschrijving* en selecteer de juiste branch op basis van het feit of je [een voorstel aan het maken bent](/processes/voorstellen-indienen.md) of [wijzigingen aan het doorvoeren bent aan een bestaand voorstel](/processes/voorstellen-wijzigen.md).

## Voeg de foto toe

Volg de instructies in [foto toevoegen](/assets/foto-toevoegen.md) om de foto gelinked in de frontmatter up te loaden. Deze foto staat best in de `_content\news\img\` folder.

## Overweeg om het nieuws item te linken in de nieuwsgrid

Volg de instructies in [newsgrid updaten](/assets/newsgrid-updaten.md) om dit te realiseren. 