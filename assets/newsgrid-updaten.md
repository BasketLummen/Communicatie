## Vereisten

Om een item in de newsgrid te plaatsen heb je 2 dingen nodig

- Een [nieuws item](/assets/newsitem-maken/)
- Een foto die vierkant is, liefst 500x500 pixels voor kleine grid items, en 1000x1000 pixels voor grote grid items. Foto's die niet vierkant zijn, te klein of te groot zijn, zullen best effort ingepast worden, maar het ziet er niet altijd goed uit.

Lees ook eerst het document over hoe je [een voorstel moet maken](/processes/voorstellen-indienen) of hoe je [wijzigingen doorvoert aan een bestaand voorstel](/processes/voorstel-wijzigen/).

## Voeg de foto toe

Volg de instructies in [foto toevoegen](/assets/foto-toevoegen) om de foto te uploaden. Deze foto staat best in de `_content\news\img\` folder.

## Wijzig de newsgrid

De inhoud van de newsgrid vind je in het bestand `\_partials\newsgrid.html`. 

Dit bestand is opgemaakt in het HTML formaat, waar elk item er als volgt uitziet:

### Items met inhoud

De meeste newsgrid items gaan inhoud hebben, voor deze items worden voorgesteld door een `div` tag met volgende inhoud:

```
<div class="newsgrid-item has-content">
	<a href="/news/de-permalink-van-een-nieuwsitem">
		<img src="/news/img/foto-naar-keuze.jpg" alt="Beschrijf de foto">
		<div class="newsgrid-item-overlay">
			<h1>De titel</h1>
			<p>Een beschrijving.</p>
			<p><span class="btn btn-lg btn-primary">Meer weten</span></p>
		</div>
	</a>
</div>
```

#### Class

Standaard zal het newsgrid item in zwart-wit renderen en 1/10de van de grid in beslag nemen, als je dit gedrag wil wijzigen kan je een class toevoegen aan de `div` tag. Bvb `<div class="newsgrid-item has-content *active*">`

* active: Dan zal het item in kleur gerendered worden.
* large: Dan zal het item 4/10e van de volledige grid in beslag nemen. Merk op dat enkel het 1e, 2e en 4e item large gemaakt mogen worden anders rendert het niet mooi op ipad's waar de grid maar 3x3 getoond kan worden. Tevens dienen items 7, 8 & 9 verwijdert te worden omdat een large item de beschikbare ruimte voor deze items inneemt.

#### Link

Het newsgrid item moet doorlinken naar de permalink van een nieuwsitem, deze permalink moet je plakken in het `href` attribuut van de `a` tag.

#### Foto

De foto wordt vertegenwoordigt door de `img` tag. In het `src` attribuut van deze tag voorzie je de link naar de gekozen foto. In het `alt` attribuut dien je de foto kort te beschrijven. Deze waarde wordt gebruikt door screen readers (voor blinden en slechtzienden).

#### Titel

De titel staat tussen de `<h1>` tags.

#### Korte beschrijving

De beschrijving staat tussen de eerste `<p>` tags. Houdt deze beschrijving kort, want op kleine schermen, zoals telefoons, overweldigt deze tekst vaak de foto.

#### Actie

Eigenlijk is heel het newsgrid item een grote knop om op te klikken, maar om mensen aan te zetten tot actie tonen we ook nog een element dat visueel op een knop lijkt. Dit is de tweede set `<p>` tags. De tekst hiervan, `Meer weten` in het voorbeeld, mag je uiteraard vervangen door iets dat thematisch meer overeenstemt met het nieuws item.

### Lege items

Wil je een item verwijderen en niks in de plaats zetten, verander dan de volledige `div` tag door onderstaande vereenvoudigde versie. Voorzie wel een leuke foto in het `src` attribuut.

```
<div class="newsgrid-item">
    <img src="/news/img/foto-naar-keuze.jpg">
</div>  
```

Het laatste item in de grid moet altijd leeg blijven, omdat dit verborgen wordt op ipads waar de grid maar 3x3 getoond kan worden.
