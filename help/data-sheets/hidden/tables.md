---
title: Tabellen
description: Werken met markeringstabellen en HTML-tabellen.
hide: true
hidefromtoc: true
exl-id: 5ce746fc-6835-4bee-85c5-5ad5176baca0
source-git-commit: 6893d1e41c3899c3ab6a9b02b305161eb3f7e049
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%

---

# Tabellen

Matt was hier telkens weer -

EDS

Standaard Markering ondersteunt alleen basistabellen. Voor AdobeDocs Markdown, hebt u de volgende opties:

* Standaardtabellen voor markeringen
* HTML-tabellen
* Markeringstabellen met een beperkte syntaxis voor alinea-einden (`<p>`), regeleinden (`<br>`) en basislijsten (`<ul>`, `<ol>`).

## HTML-tabellen converteren naar markeringstabellen

In sommige gevallen wilt u een HTML-tabel omzetten in een Markeringen of in Markeringen. Mogelijk moet u de weergave verbeteren, een validatiefout oplossen of het makkelijker maken om de bewerking verder uit te voeren.

Helaas, hebben wij geen enkel hulpmiddel kunnen vinden dat HTML lijsten goed omzet. Doorgaans gebruiken we een combinatie van tools om een fatsoenlijke prijsopgave samen te voegen.

| Tool | Wat doet het? |
|--- |--- |
| [ de Generator van Lijsten van de Vermindering ](https://www.tablesgenerator.com/markdown_tables) | Goed voor het maken van geheel nieuwe opmaak voor tabellen. |
| [ Geavanceerde lijstomzetter ](https://tableconvert.com/html-to-markdown) | Tabellen converteren van elke indeling naar elke gewenste indeling. <p>**Nota:** de Verbindingen en de beelden worden afgevlakt wanneer omgezet. |
| [ Basis lijst html > telleromzetter ](https://jmalarcon.github.io/markdowntables/) | Eenvoudige HTML-converter <p>**Nota:** de Verbindingen en de beelden worden afgevlakt wanneer omgezet. |
| [ niet-lijst HTML > de omzetter van de Prijsonderdruk ](https://codebeautify.org/html-to-markdown) | Hiermee converteert u HTML-tabellen naar niet-tabelmarkeringssyntaxis. In combinatie met de bovenstaande gereedschappen gebruiken voor het kopiëren van koppelingen, afbeeldingen en andere samengevoegde items. |

## Standaardtabellen voor markeringen

* Zorg ervoor dat u ten minste drie afbreekstreepjes toevoegt in de tweede rij die de tabeleigenschappen bepaalt. Voorbeeld: `|--- |--- |--- |` voor een tabel met drie kolommen.
* Markeringstabellen moeten ten minste één koptekstrij en één tekstrij hebben. U kunt geen één rij of één-cel markeringstabel tot stand brengen (gebruik in plaats daarvan HTML).
* Zorg ervoor dat elke rij hetzelfde aantal verticale strepen (&vert;) tekens bevat. Als u een pijpkarakter binnen een lijstcel moet omvatten, escape door het met backslash (`\|`) of het gebruiken van de de entiteitcode van de HTML (`&vert;`) vóór te gaan.
* Wees voorzichtig met het gebruik van codeblokken in tabellen. Inline-codeblokken kunnen leiden tot onevenredige kolombreedten.
* U kunt de weergave van de tabel wijzigen door Automatisch of Vast op te geven. Zie [ Veranderend hoe de lijsten ](#table-rendering) worden teruggegeven.

## Opmaaktabellen maken met bonus HTML

Om migratie te vergemakkelijken, hebben wij de lijsten van de Prijsverhoging uitgebreid om HTML paragraafonderbrekingen (`<p>`), lijnonderbrekingen (`<br>`), en basislijsten van de HTML (`<ul>` en `<ol>`) binnen de lijsten van de Prijsverhoging te steunen.

**de lijst van de Prijsverhoging met lijnonderbrekingen en lijsten**

```
| Header 1 | Header 2 | Header 3 |
|--- |--- |--- |
| Normal row | row 1 column 2 | row 1 column 3 |
| Line break | first line in cell<br>second line in cell | row 1 column 3 |
| Bullet list | Bullet list:<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul> | row 2 column 3 |
| Bullet list with line break | Bullet list:<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul><br>This is a new line after the bullet list | row 2 column 3 |
```

**Voorbeeld**

| Koptekst 1 | Koptekst 2 | Koptekst 3 |
|--- |--- |--- |
| Normale rij | rij 1 kolom 2 | rij 1 kolom 3 |
| Regeleinde | eerste lijn in cel <br> tweede lijn in cel | rij 1 kolom 3 |
| Lijst met opsommingstekens | Lijst met opsommingstekens:<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul> | rij 2 kolom 3 |
| Lijst met opsommingstekens met regeleinde | Lijst met opsommingstekens:<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul><br> Dit is een nieuwe lijn na de bulletlijst | rij 2 kolom 3 |

>[!IMPORTANT]
>
>Als u besluit om HTML in inheemse lijsten te gebruiken, zorg ervoor dat u juiste syntaxis van de HTML gebruikt. Fouten in de syntaxis van HTML resulteren in validatiefouten die moeilijk te begrijpen zijn. Controleer uw werk.

## Werken met HTML-tabellen

Het migratiehulpmiddel probeerde om zo veel mogelijk het formatteren van de originele lijst te bewaren. Het grootste deel van deze syntaxis van HTML wordt genegeerd, terwijl sommige van deze syntaxis in bevestigingsfouten resulteert.

**Steekproef gemigreerde HTML lijst**

```
<table> 
 <tbody>
  <tr>
   <th>Property</th> 
   <th>Type</th> 
   <th>Value Description</th> 
  </tr>
  <tr>
   <td>badgingPath</td> 
   <td>String[]</td> 
   <td><p><i>(Required)</i> A multi-value string of badge images up to the number of badgingLevels. The badge image paths must be ordered so the first is awarded to the highest expert. If there are less badges than indicated by badgingLevels, the last badge in the array fills out the rest of the array. Example entry:</p><p> <code>/etc/community/badging/images/expert-badge/jcr:content/expert.png</code></p></td> 
  </tr>
  <tr>
   <td>badgingLevels</td> 
   <td>Long</td> 
   <td><i><p>(Optional)</i> Specifies the levels of expertise to be awarded. For example, if there should be an <code>expert </code>and an <code>almost expert</code> (two badges), then the value should be set to 2. The badgingLevel should correspond with the number of expert-related badge images listed for the badgingPath property. Default is 1.</p></td> 
  </tr>
  <tr>
   <td>badgingType</td> 
   <td>String</td> 
   <td><p><i>(Required)</i> Identifies the scoring engine as either "basic" or "advanced". Set to "advanced" else the default is "basic".</p></td> 
  </tr>
 </tbody>
</table>
```

**teruggegeven**

<table> 
 <tbody>
  <tr>
   <th>Eigenschap</th> 
   <th>Type</th> 
   <th>Beschrijving van waarde</th> 
  </tr>
  <tr>
   <td>badgingPath</td> 
   <td>String[]</td> 
   <td><p><i> (Vereist) </i> Een multi-waardekoord van badge beelden tot het aantal badgingLevels. De wegen van het badge beeld moeten worden bevolen zodat wordt de eerste toegekend aan de hoogste deskundige. Als er minder badges zijn dan aangegeven door badgingLevels, vult het laatste badge in de array de rest van de array in. Voorbeeld:</p><p> <code>/etc/community/badging/images/expert-badge/jcr:content/expert.png</code></p></td> 
  </tr>
  <tr>
   <td>badgingLevels</td> 
   <td>Lang</td> 
   <td><p><i> (Facultatief) </i> specificeert de niveaus van deskundigheid te gunnen. Als er bijvoorbeeld een <code>expert </code> en een <code>almost expert</code> (twee badges) moeten zijn, moet de waarde worden ingesteld op 2. Het badgingLevel moet overeenkomen met het aantal deskundige badge-afbeeldingen dat voor de eigenschap badgingPath wordt vermeld. De standaardwaarde is 1.</p></td> 
  </tr>
  <tr>
   <td>badgingType</td> 
   <td>String</td> 
   <td><p><i> (Vereist) </i> identificeert de het scoring motor als of "basis"of "geavanceerd". Ingesteld op "advanced" anders is de standaardwaarde "basic".</p></td> 
  </tr>
 </tbody>
</table>

**wanneer om HTML lijsten** te gebruiken

* Kolommen in evenwicht brengen.
* Tabelkoppen weglaten (voor markeringstabellen moet een koptekstrij zijn vereist).
* Om de grens van een één-rij lijst (`<tr style="border: 0;">`) te verwijderen.
* Kolom- of rijbereiken toevoegen.
* Tekst in een tabelcel uitlijnen.

**Nota&#39;s voor het werken met HTML lijsten**

* Gebruik geen Markeringen in HTML-tabellen. Als u bijvoorbeeld `[!NOTE]` toevoegt aan een HTML-tabel, wordt deze weergegeven zoals (`[!NOTE]`). Gebruik in plaats daarvan de syntaxis HTML voor bijvoorbeeld notities en afbeeldingen.

  Loc-tags vormen een uitzondering op deze regel, omdat UICONTROL- en DNL-tags worden verwijderd voordat de pagina&#39;s worden weergegeven.

* Niet alle syntaxis van de HTML wordt ondersteund in tabellen. Breedte, hoogte, kleur en andere HTML-syntaxiselementen worden genegeerd wanneer deze worden gerenderd in EXL. U kunt deze waarden in laten, tenzij deze resulteren in validatiefouten.
* Als u tekst wilt uitlijnen, gebruikt u `align: "left|center|right"` in HTML. Als u bijvoorbeeld de inhoud van een tabelcel wilt centreren, gebruikt u `<td align="center">` .
* HTML-tabellen kunnen geen geneste tabellen bevatten.

>[!TIP]
>
>Als u een rand voor een HTML-tabel met één rij wilt uitschakelen, gebruikt u deze syntaxis:
>
>```
><table>
><tr style="border: 0;">
>```

## Opgeven hoe tabellen worden gerenderd {#table-rendering}

U kunt tabellen op twee manieren weergeven:

* **Vast** (momenteel het gebrek) - omvat douaneregels voor het teruggeven van lijsten, met inbegrip van HTML lijsten met beelden. Tabellen worden gerenderd als volledige-breedte zonder schuiven, wat soms overlappende tekst veroorzaakt.
* **Auto** - Gelijkaardig aan Git-Gantsmaakte Markering (GFM). Tabellen mogen schuiven, zodat de tekst niet overlapt.

In de meeste gevallen worden de tabellen weergegeven met dezelfde weergave. Als uw tabel echter overlappende tekst bevat, wilt u de tag `auto` toepassen. Als de HTML-tabel met afbeeldingskaarten niet correct wordt weergegeven, wilt u mogelijk de tag `fixed` toepassen.

We overwegen de standaardinstelling te wijzigen van `fixed` in `auto` .

## Markeringstabellen bewerken

Als u wilt specificeren hoe een inheemse markeringslijst wordt teruggegeven, voeg één van deze syntaxislijnen na de lijst, met lege lijnen voor en na toe:

* `{style="table-layout:auto"}`
* `{style="table-layout:fixed"}`

![ lijst-teruggevend ](assets/table-render.png)

### HTML-tabellen bewerken

Als u wilt specificeren hoe een HTML lijst wordt teruggegeven, gebruik één van deze syntaxislijnen in de eerste lijn van de lijst:

* `<table style="table-layout:auto">`
* `<table style="table-layout:fixed">`

```
<table style="table-layout:fixed">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```

### Wanneer gebruikt u Automatisch of Vast

**Overlappende tekst**

Gebruik `auto` voor tabellen met lange codeblokken of tekst die overlappende tekst veroorzaakt wanneer `fixed` (standaardwaarde) is geselecteerd.

*Vast (Gebrek)*

| Metrische informatie | Beschrijving | ID-queryparameter |
| ---- | ---- | ---- |
| **timeseries.data.collection.validation.category.type.count** | Het totale aantal ongeldige &quot;type&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.range.count** | Het totale aantal ongeldige &quot;waaier&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.format.count** | Het totale aantal ongeldige &quot;formaat&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.pattern.count** | Het totale aantal ongeldige &quot;patroon&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.presence.count** | Het totale aantal ongeldige &quot;aanwezigheid&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.enum.count** | Het totale aantal ongeldige &quot;enum&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |

{style="table-layout:fixed"}

*Auto*

| Metrische informatie | Beschrijving | ID-queryparameter |
| ---- | ---- | ---- |
| **timeseries.data.collection.validation.category.type.count** | Het totale aantal ongeldige &quot;type&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.range.count** | Het totale aantal ongeldige &quot;waaier&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.format.count** | Het totale aantal ongeldige &quot;formaat&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.pattern.count** | Het totale aantal ongeldige &quot;patroon&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.presence.count** | Het totale aantal ongeldige &quot;aanwezigheid&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |
| **timeseries.data.collection.validation.category.enum.count** | Het totale aantal ongeldige &quot;enum&quot;berichten voor één dataset of voor alle datasets. | Dataset-id |

{style="table-layout:auto"}

**HTML lijsten met evenwichtige beelden**

Gebruik `fixed` voor HTML-tabellen waarvoor evenwichtige afbeeldingen nodig zijn die onevenwichtig worden wanneer `auto` wordt geselecteerd. In dit voorbeeld hebben de afbeeldingen dezelfde grootte, maar de middelste kolom bevat meer tekst.

*Auto*

<table style="table-layout:auto">
<tr>
  <td>
    <a href="note-test.md">
    <img alt="Lood" src="assets/leads-home.png"/>
    </a>
    <div>
    <a href="note-test.md"><strong> Werkschema voor Adobe leidt </strong></a>
    </div>
    <em> Belangrijkste het uitgeven werkschema voor loodschrijvers.</em>
    <br>
  </td>
  <td>
    <a href="syntax-style-guide.md">
      <img alt="Onfrequent" src="assets/infrequent.png">
    </a>
    <div>
    <a href="syntax-style-guide.md"><strong> Werkschema voor Onfrequente Gebruikers </strong></a>
    </div>
    <em> geen leidende schrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de gemakkelijkste manieren om bijdragen te maken.</em>
    <br>
  </td>
  <td>
    <a href="note-test.md">
      <img alt="Validatie" src="assets/validation.png">
    </a>
    <div>
    <a href="note-test.md"><strong> Bevestiging </strong></a>
    </div>
    <em> Leer om bevestigingsfouten op te lossen.</em>
    <br>
  </td>
</tr>
</table>

*Vast (op meer manieren dan één)*

<table style="table-layout:fixed">
<tr>
  <td>
    <a href="note-test.md">
    <img alt="Lood" src="assets/leads-home.png"/>
    </a>
    <div>
    <a href="note-test.md"><strong> Werkschema voor Adobe leidt </strong></a>
    </div>
    <em> Belangrijkste het uitgeven werkschema voor loodschrijvers.</em>
    <br>
  </td>
  <td>
    <a href="syntax-style-guide.md">
      <img alt="Onfrequent" src="assets/infrequent.png">
    </a>
    <div>
    <a href="syntax-style-guide.md"><strong> Werkschema voor Onfrequente Gebruikers </strong></a>
    </div>
    <em> geen leidende schrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de eenvoudigste manieren om bijdragen te leveren. Geen hoofdschrijver? Leer de gemakkelijkste manieren om bijdragen te maken.</em>
    <br>
  </td>
  <td>
    <a href="note-test.md">
      <img alt="Validatie" src="assets/validation.png">
    </a>
    <div>
    <a href="note-test.md"><strong> Bevestiging </strong></a>
    </div>
    <em> Leer om bevestigingsfouten op te lossen.</em>
    <br>
  </td>
</tr>
</table>
