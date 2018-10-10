Iedereen kan voorstellen indienen voor wijzigingen aan de inhoud van de website (of eender welke andere repository op github). De enige vereiste is dat je een github account hebt, indien je die nog niet hebt kan je op https://github.com/join een gratis account aanmaken.

## Inhoud wijziging maken

Eerst en vooral dien je de inhoud, van je voorstel tot wijziging, te maken. Dit is buiten de scope van dit document, maar hier kan je een aantal handleidingen vinden van de meest voorkomende wijzigingen:

* [Nieuws item maken voor website](/assets/newsitem-maken.md)
* [Een foto toevoegen aan de website](/assets/foto-toevoegen.md)
* [De newsgrid updaten](/assets/newsgrid-updaten.md)

## Maak een branch

Eens de inhoud van je voorstel klaar is, dien je deze aan te bieden als een zogenaamde Pull Request. Dit proces is verschillend afhankelijk van het feit of je rechten hebt op de repository of niet.

### Indien je wel rechten hebt

Dan realiseer je dit door onderaan een wijzigings pagina in de *Commit Changes* sectie de optie *`Create a new branch for this commit and start a pull request`* te selecteren.

In de eerste stap maken we een branch met 1 wijziging aan. Een branch stelt een bepaalde toekomstige versie van de inhoud voor, maar binnen de repository, deze geef je best een *betekenisvolle naam*, in het formaat `de-door-jouw-gekozen-branch-naam`. 

In de velden erboven dien je een *betekenisvolle titel* en *beschrijving* te geven. 

Deze titel en beschrijving horen bij de voorgestelde wijziging. Een Pull Request kan meerdere wijzigingen omvatten, dit is de eerste, je kan later nog wijzigingen toevoegen.

Daarna druk je op de groene knop met de tekst *Propose file change* of gelijkaardig. 

### Indien je geen rechten hebt

Dan heb je onderaan een wijzigings pagina geen opties en zal er altijd een zogenaamde `Fork` aangemaakt worden met daarin een nieuwe branch.
Een `Fork` is een volledige copy van de hele repository, waar een `branch` slechts een copy is van een tak, maar nog binnen dezelfde boomstructuur. De naam van deze branch kan je helaas niet kiezen, hij heet altijd `patch-nummer`.

In de invulvelden dien je een *betekenisvolle titel* en *beschrijving* te geven. 

Deze titel en beschrijving horen bij de voorgestelde wijziging. Een Pull Request kan meerdere wijzigingen omvatten, dit is de eerste, je kan later nog wijzigingen toevoegen.

Daarna druk je op de groene knop met de tekst *Propose file change* of gelijkaardig. 

## Maak de pull request

Op de volgende pagina ga je de pull request zelf aanmaken.

Links bovenaan, net onder *Open a pull request* zie je, als je rechten hebt, 2 dropdowns. Zorg ervoor dat in de eerste `master` staat en in de tweede `de-door-jouw-gekozen-branch-naam`

Indien je vanuit een `Fork` werkt, als je geen rechten had op de originele repository, dan gaat het over de 2e en de 4e dropdown, de 1e en 3e bevatten de namen van de respectievelijke forks. In dit geval moet je ook eerst op de groene knop `Create pull request` clicken vooraleer de invulvelden verschijnen.

In deze velden dien je opnieuw een *betekenis volle titel* en *beschrijving* te voorzien. Standaard wordt dit ingevuld met dezelfde tekst als je ingegeven hebt op de eerste wijziging. 

Als dit de enige wijziging is, dan is dit waarschijnlijk voldoende. 

Als je van plan bent nog extra wijzigingen door te voeren in dit voorstel, dan beschrijf je hier best het volledig plaatje. In dit geval voeg je ook best de tekst `[WIP]` toe vooraan in de titel. Zo weten de reviewers dat de inhoud nog een *Work in progress* is.

Wanneer je klaar bent met beschrijven, dan klik je op de groene knop *Create pull request*.

## Duid reviewers aan

De volgende pagina die je krijgt is bedoeld om de inhoud te reviewen en te discussieren over het voorstel indien nodig.

Om dit makkelijker te maken, selecteer je in de rechter bovenhoek de `Reviewers`. De mensen die je hier aanduid zullen een bericht krijgen dat je pull request klaar is voor review.

Eventuele commentaren kan je onderaan deze pagina toevoegen.

Bij deze ben je klaar en kan het review proces beginnen.