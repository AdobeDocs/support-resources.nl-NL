---
title: Self Service Excellence Collaborative Documentation Syntax and Formatting Guide
description: Een basisinleiding tot opmaak van markeringen
mini-toc-levels: 1
hide: true
hidefromtoc: true
source-git-commit: e2513757c4d126e0ab954b05002392aaa4ed46c8
workflow-type: tm+mt
source-wordcount: '4237'
ht-degree: 0%

---

# Handleiding voor syntaxisstijl voor opmaak

Deze pagina illustreert de onderdrukkingscomponent voor Digital Experience Technical Documentation Authoring aan de hand van de opmaak .md (markdown). Deze pagina bevat gegevens voor medewerkers van Adoben.

Zie hier: [Adobe.com](https://www.adobe.com){rel=nofollow}

<!--
* You can [view a basic sample file](sample.md) or [view a sample file with advanced syntax examples](sample-full.md)
-->

>[!TIP]
>
>Dit bekijken [Video over AdobeDocs Markdown](https://video.tv.adobe.com/v/26165).

Voor het grootste deel, volgen wij standaard git-gearomatiseerde prijsingssyntaxis (GFM) voor het formatteren van tekst. Nochtans, wordt sommige syntaxis (zoals horizontale lijnen) niet gesteund, en wij hebben Markdown op een aantal manieren uitgebreid om onze documentatiebehoeften aan te passen.

## Basistekstopmaak

Een alinea vereist geen speciale syntaxis in Markdown. Voeg een lege regel toe tussen elke alinea.

Tekst opmaken als **vet**, plaatst u deze in twee sterretjes:

```
This text is **bold**.
```

Tekst opmaken als *cursief*, plaatst u deze in één sterretje:

```
This text is *italic*.
```

Tekst opmaken als beide ***vet en cursief***, plaatst u deze in drie sterretjes:

```
This is text is both ***bold and italic***.
```

Als u opmaaktekens voor markeringen wilt negeren, gebruikt u `\` vóór het teken:

`This is not \*italicized\* type.`

Gerenderd: dit type is niet \*cursief\*.

## Badges

In uitvoering. Wachten op loc.

<!--

See the [dev version of this article](https://experienceleague-dev.corp.adobe.com/docs/authoring-guide-exl/using/markdown/syntax-style-guide.html#badges) for an example. Or [this one](https://experienceleague-dev.corp.adobe.com/docs/internal-test/test/badge.html).

There are two ways to create badges:

* **Metadata badge** - Specify the badge information in metadata so that the badge appears above the title in the article. This is especially useful for adding a badge to all articles in a guide or repo via the TOC.md or metadata.me files.
* **Inline badge** - Specify the badge information on its own line or in a heading, table, or other page element.

![badge examples](assets/badge-examples.png)

**Badge syntax**

*Metadata*: `badge: "Beta Content" type="Informative" url="https://www.example.com" tooltip="Go to example.com"`

*Inline*: `[!BADGE Beta Content]{type=Informative url="https://www.example.com" tooltip="Go to example.com"}`

**Examples**

```
|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Maybe]{type=Neutral tooltip="A rider fell off his horse..."}|
|Caution|[!BADGE Attention]{type=Caution tooltip="Yellow status"}|
```

**Rendered**

|Type|Badge|
|---|---|
|Informative (default)|[!BADGE Beta]{type=Informative url="https://www.example.com"}|
|Positive|[!BADGE New Feature]{type=Positive url="https://www.example.com" tooltip="Go to example.com"}|
|Negative|[!BADGE Discontinued]{type=negative tooltip="This feature is now end of life"}|
|Neutral|[!BADGE Maybe]{type=Neutral tooltip="A rider fell off his horse..."}|
|Caution|[!BADGE Attention]{type=Caution tooltip="Yellow status"}|

**More details**

* Only the badge label is required. The `type`, `url`, and `tooltip` parameters are optional. The `type` parameter determines the color. The `url` parameter lets users click the badge to open an article. The `tooltip` parameter displays the tooltip text on mouseover.
* If you want multiple badges to appear at the top of the page, use different badge names. For example, you can create badge names such as `badgeBeta` or `badgeWeb`. Example:

  ```
  badge1: "Beta"
  badge2: "Campaign Web"
  ```

* For metadata badges, make sure that all values are wrapped in quotes. For inline badges, make sure that `url` and `tooltip` are wrapped in quotes.
* Valid type values include *Informative* (default, blue), *Positive* (green), *Negative* (red), *Neutral* (dark gray), and *Caution* (yellow). 

-->

## Blokkeringen

Ons ontwerpsysteem gebruikt blockquotes (`>` aan het begin van regels) om aangepaste markeringsextensies te identificeren voor tips, notities en video&#39;s. U kunt echte blockquotes maken door een `>` vóór een alinea.

>Dit is een blockquote.

```
>This is a blockquote quotation.
```

## Codeblok (op regel){#code-block}

**Wanneer gebruiken**

Wordt gebruikt om een stukje code in een zin online weer te geven. Ideaal om een cookie-naam, bestandsnaam, waarde of opdracht op te roepen waarvoor geen codeblok met volledige omtrek vereist is.

Inhoud binnen codeblokken in rendering as is and not localized. (De enige uitzondering op deze regel is `!UICONTROL` en `!DNL` syntaxis, die wordt verwijderd tijdens het maken van het pakket.)

Gebruik ook codeblokken voor voorbeeld-URL&#39;s die niet moeten worden gevalideerd: `https://www.example.com`

**Syntaxis**

Een codeblok gebruikt één enkele backticks om het code-element te omsluiten u zou willen benadrukken.

```
This is `inline code` within a paragraph of text.
```

**Voorbeeld**

Dit is `inline code` in een alinea met tekst.

>[!TIP]
>
>U kunt tekst ook in drievoudige achtertikken (&grave;&grave;&grave;) laten omlopen om een inline-codeblok te maken. Dit is vooral nuttig wanneer u een achtertikteken binnen een gealigneerd codeblok moet van verwijzingen voorzien. Voorbeeld:
>
&grave;&grave;`Use a back tick (`&amp;graf;`) for formatting`&grave;&grave;

## Codeblok (afgezonderd)

**Wanneer gebruiken**

Gebruik een codeblok om de syntaxis van de code weer te geven. Een omheind codeblok gebruikt drie keer de achtergronden om het code-element dat u wilt markeren, te omsluiten. Voeg lege regels toe boven en onder het omheinde codeblok.

Codeblokken zijn niet gelokaliseerd.

>[!TIP]
>
Geef een taal op wanneer u een omheind codeblok maakt. Als u een taal opgeeft, is syntaxismarkering mogelijk die specifiek is voor die taal en wordt een **Kopiëren** voor de gebruikers. U kunt ook regelnummers weergeven als u een taal opgeeft.

**Syntaxis**

Gebruik drie achtertikken (&grave;&grave;&grave; ) voor en na de coderegels. Zorg ervoor dat de open en dichte achtertikken hetzelfde aantal spaties inspringen. Geef een codetaal op voor optimale rendering.

&grave;&grave;`javascript`

**Voorbeeld**

```javascript
var visitor = Visitor.getInstance("INSERT-MARKETING-CLOUD-ORGANIZATION ID-HERE", {
     trackingServer: "INSERT-TRACKING-SERVER-HERE", // same as s.trackingServer
     trackingServerSecure: "INSERT-SECURE-TRACKING-SERVER-HERE", // same as s.trackingServerSecure

     // To enable CNAME support, add the following configuration variables
     // If you are not using CNAME, DO NOT include these variables
     marketingCloudServer: "INSERT-TRACKING-SERVER-HERE",
     marketingCloudServerSecure: "INSERT-SECURE-TRACKING-SERVER-HERE" // same as s.trackingServerSecure
});
```

### Syntaxis markeren voor codeblokken

Experience League ondersteunt syntaxismarkering voor codeblokken. Zorg ervoor dat u een taal opgeeft, zoals `java` na de openingsreeks tikken om ervoor te zorgen dat de syntaxis behoorlijk wordt benadrukt. Zie voor een lijst met geldige talen [https://prismjs.com](https://prismjs.com/#supported-languages). Als er talen ontbreken, registreert u een jira-ticket.

### Regelnummering in codeblokken

Toevoegen `{line-numbers="true"}` na de taal om regelnummering in te schakelen.

Voorbeeld met regelnummers (&grave;&grave;&grave;`html {line-numbers="true"}`):

```html {line-numbers="true"}
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

**Nummering beginnen op regel _**

Toevoegen `start-number="n"` na de syntaxis van het regelnummer om de nummering te laten beginnen op een ander nummer dan 1.

Voorbeeld met nieuwe beginregel (&grave;&grave;&grave;`html {line-numbers="true" start-line="7"}`):

```html {line-numbers="true" start-line="7"}
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>
<p>My second paragraph.</p>

</body>
</html>
```

### Regelmarkering in codeblokken

Toevoegen `highlight="n"` na de syntaxis van het regelnummer om rijen binnen een codeblok te markeren. Opgeven `11-13, 16` worden de lijnen 11 tot en met 13 en 16 benadrukt.

Voorbeeld met lijnmarkering (&grave;&grave;&grave;`html {line-numbers="true" start-line="7" highlight="11-13, 16"}`):

```html {line-numbers="true" start-line="7" highlight="11-13, 16"}
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>
<p>My second paragraph.</p>

</body>
</html>
```

### Variabele opmaak in codeblokken

Variabele syntaxis, zoals `<i>italic</i>` wordt niet ondersteund in codeblokken. U kunt de tekst van een variabele aangeven door de punthaken te gebruiken `< >`.

## Inklapbare secties

U kunt een inklapbare sectie maken (ook wel een **accordeon**) die standaard verborgen is. De gebruiker kan op de titel klikken om de sectie uit of samen te vouwen.

Inklapbare tekst kan worden gebruikt om complexe inhoud te vereenvoudigen, zoals het stroomlijnen van een pagina met veelgestelde vragen of het decompileren van een complexe procedure met geneste lijsten. In plaats van bijvoorbeeld een set substappen weer te geven, kunt u de substappen samenvouwen tot een sectie &#39;Details weergeven&#39;.

**Syntaxis**

```
+++See details
This is text inside a collapsible section.

* Bullet one
* Bullet two
* Bullet three

+++
```

**Voorbeeld**

+++Zie details Dit is tekst binnen een inklapbaar gedeelte.

* Opsommingsteken
* Opsommingsteken twee
* Opsommingsteken drie

+++

**Notities**

* U mag geen inklapbare secties nesten binnen inklapbare secties. Geneste inklapbare secties worden niet goed gerenderd. Nochtans, veroorzaken zij geen bevestiging om te ontbreken, zodat zullen de gebruikers zien `+++` syntaxis van de geneste sectie.
* Zorg ervoor dat u lege regels boven en onder items zoals opsommingstekens en codeblokken binnen de inklapbare sectie toevoegt, of u krijgt een validatiefout.
* U kunt koppen toevoegen binnen inklapbare secties, maar dit wordt niet aanbevolen.
* [Accordeons zijn niet altijd het antwoord op complexe inhoud op desktops](https://www.nngroup.com/articles/accordions-complex-content/)
* Een historisch nadeel van inklapbare gedeelten is dat **Zoeken in pagina** (Ctrl/Cmd+F) Samengevouwen tekst wordt genegeerd. In Safari is dat nog steeds het geval, maar in Chrome is dat niet meer het geval. Met Zoeken in pagina wordt samengevouwen tekst in Chrome gedetecteerd.
* Voorbeeld van een [onderhoudsupdates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en) pagina met inklapbare secties.

## Opmerkingen en opmerkingen

Opmerkingen worden niet weergegeven in het weergegeven Help-systeem. Opmerkingen gebruiken om opmerkingen voor uzelf of andere schrijvers te achterlaten. U kunt ook opmerkingen gebruiken voor conceptsgedeelten.

Houd er voor opmerkingen rekening mee dat deze niet worden weergegeven in het Help-systeem, maar wel zichtbaar zijn voor gebruikers die Markeringen bewerken op GitHub.com. Vertrouwelijke informatie niet opnemen in opmerkingen.

```
<!-- standard comment code -->

DO NOT USE the following:
<!--> bad comment syntax <-->
```

U moet de tekst hieronder niet kunnen zien (&quot;U kunt me niet zien&quot;) tenzij u het document bewerkt.

<!--
You can't see me (unless you're editing in Git).
-->

**Herinnering:** Opmerkingen (opmerkingen) worden niet weergegeven in de voor het publiek toegankelijke Help-artikelen. Opmerkingen worden echter wel weergegeven in de openbare opmaakbestanden die gebruikers kunnen zien en bewerken.

>[!IMPORTANT]
>
Voeg geen opmerkingen toe aan blokcomponenten, zoals lijsten met opsommingstekens, vooral geneste lijsten met opsommingstekens. De opmerking kan de manier wijzigen waarop de lijst met opsommingstekens wordt weergegeven.
>
Plaats in het bestand TOC.md geen opmerkingen over regels in het midden van de lijst met inhoudsopgave. Hierdoor kan de lijst met inhoudsopgaven worden verbroken en kunnen validatiefouten optreden. Verplaats in plaats daarvan opmerkingen in de inhoudsopgave naar het einde van het bestand.

## CONTEXTUALHELP

Auteurs kunnen met productteams werken om hulppopovers in de Experience Cloud of het product UI van de Experience Platform toe te voegen. Voorbeeld:

```markdown
>[!CONTEXTUALHELP]
>id="platform_destinations_activate_mandatorykey_4"
>title="About mandatory attributes"
>abstract="Select the XDM schema attributes that all exported profiles should include. Profiles without the mandatory key are not exported to the destination. Not selecting a mandatory key exports all qualified profiles regardless of their attributes."
>additional-url="http://www.adobe.com/go/destinations-mandatory-attributes-en" text="Learn more in documentation"
```

## Definitielijsten

Voor definitielijsten, steunen wij nog geen standaardsyntaxis van de Prijsverhoging. Gebruik in plaats daarvan de volgende handmatige opmaak:

```
**Frog** - An amphibious green creature. Likes flies.
```

Gerenderd:

**Kikker** - Een amfibieus groen schepsel. Likes vliegt.

<!--
A definition list is a Markdown extension that supports the Definition List component in AEM. A definition list consists of a term and its definition.

**When to use**

Using a definition list is optional. To define lists of features or options, you can use either the definition list syntax or use basic Markdown formatting, such as applying bold to option names.

**Syntax**

```
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

**Example**

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
-->

## Bestanden downloaden

Upload het .zip- of ander downloadbaar bestand naar de map assets en koppel er vervolgens aan. Als het een ZIP-bestand is, wordt het bestand gedownload wanneer u op de koppeling klikt. Als het bestandstype bijvoorbeeld PDF of PNG is dat in een browser kan worden geopend, wordt door op de koppeling te klikken een nieuw tabblad geopend. Voor dergelijke bestanden kunt u overwegen ze te comprimeren of instructies geven om met de rechtermuisknop op de koppeling te klikken en te downloaden.

`Download` &amp;lbrack;`download-test.zip`&amp;rek;`(assets/download-test.zip)`

Gerenderd:

Downloaden [download-test.zip](assets/download-test.zip)

>[!NOTE]
>
De maximale bestandsgrootte voor het downloaden van bestanden en afbeeldingen is 100 MB. Dat is de github.com-limiet. De limiet voor git.corp.adobe.com is hoger (250 MB), maar we moeten bestanden kunnen kopiëren naar de spiegel github.com.

## Koppen {#headings}

In Markering gebruikt u hekje (`#`) om de kopniveaus te identificeren. Het eerste niveau (`#`) is de titel van het artikel, die ook is opgegeven in de metagegevenskop. Houd deze dezelfde titel aan. Het tweede niveau (`##`) staat voor de belangrijkste koppen op de pagina die in de miniinhoudsopgave worden opgenomen. Als u gewend bent om in AEM te schrijven (chl-auteur), de niveau 2 rubrieken (`##`) aan de component &quot;Kop 1&quot; in AEM.

Maximum aantal tekens voor koppen: 69 tekens (Engels) / 120 tekens (LOC).

```
# This is level 1 (article title)

## This is level 2
   
### This is level 3
```

**Best practices voor kopteksten**

* Zorg ervoor dat een kop van niveau 1 (`#`) volgt een lege regel na de metagegevens in elk artikel.
* Niveaus niet overslaan, zoals van niveau 2 springen (`##`) tot niveau 4 (`####`).
* Een lege regel opnemen *voor* en *na* elke rubriek.
* Als een kop cijfers bevat, geeft u een expliciete kop-id op die niet met een getal begint, zoals `## Release notes for 2016 {#release-notes-2016}`.
* We raden slechts drie niveaus aan. Niveaus 4 en hoger worden op dit moment niet correct weergegeven.
* Koppen worden weergegeven in de rechternav, zodat gebruikers kunnen klikken om naar een sectie te gaan. Standaard worden twee niveaus van koppen weergegeven in de rechternav. Als u het aantal niveaus wilt wijzigen, gebruikt u `mini-toc-levels` metagegevens, zoals `mini-toc-levels: 3`.

**Kop-id&#39;s**

Kop-id&#39;s (ook wel *anker-id&#39;s*) worden gebruikt om aangepaste diepgaande koppelingen naar secties in artikelen te maken. Gebruik de volgende notatie om een kop-id op te geven:

```
## Creating processing rules {#processing-rules}
```

Kop-id&#39;s moeten in kleine letters worden weergegeven en worden afgebroken.

Als u geen kop-id opgeeft voor een kop, is de standaardkop-id de kop &#39;Gegraveerd&#39; (kleine letters en afgebroken). Bijvoorbeeld de `## Creating widgets and Such` koptekst bevat een `#creating-widgets-and-such` anker.

## HTML-syntaxis {#html}

Om verschillende redenen, zoals veiligheid en toegankelijkheid, beperken wij de syntaxis van de HTML die in prijsvermindering kan worden gebruikt. In de volgende lijst ziet u de ondersteunde HTML-syntaxis. Elke syntaxis van de HTML die niet in deze lijst staat, resulteert in een validatiefout.

```html
<table>
<tbody>
<td>
<tfoot>
<thead>
<th>
<tr>
<col>
<colgroup>
<p> (paragraph break)
<ul> (unordered list / numbered list)
<ol> (ordered list / bullet list)
<li> (list item)
<br> (line break)
<b>
<caption>
<i>
<strong> (bold)
<u> (underline)
<s> (strikethrough)
<span>
<sub> (subscript)
<sup> (superscript)
<a>
<img>
<div>
<em> (emphasis, italics)
<pre> (codeblock)
<code>
<codeblock>
```

<!--
Bob: Check above no space char. (ignore the space; I can't add a codeblock inside this codeblock)
-->

Als u de syntaxis van de HTML aan deze lijst wilt worden toegevoegd, gelieve een kaartje te registreren of het SSE team te contacteren.

## Afbeeldingen {#images}

Gebruik de `![]()` syntaxis voor afbeeldingen. De vierkante haken `[ ]` alt-tekst en de haakjes opnemen `( )` De locatie van de afbeelding en optionele aanwijstekst (knopinfo). Met het uitroepteken wordt een afbeelding onderscheiden van een koppeling.

```
![alt text](assets/logo.png "Hover text")
```

![alt-tekst](assets/logo.png "Tekst boven")

Voor gedeelde afbeeldingen kunt u de afbeeldingen in een map met hoofdmiddelen plaatsen en vervolgens een hoofdkoppeling gebruiken die vanuit elk bestand in een repo werkt:

```
/help/assets/imagename.png
```

### Afbeeldingen vergroten/verkleinen en uitlijnen

**Afbeeldingseigenschappen (met rechts uitgelijnde afbeelding)** ![alt-tekst](assets/premium.png "Premium-aanwijstekst"){align="right"}

Gebruik bijvoorbeeld de volgende syntaxis om de standaardafbeeldingsbreedte te wijzigen of de afbeelding in de paginaweergave of tabelcel te centreren of rechts uit te lijnen.

```
![Dive image alt text](assets/maui-dive.jpg "Hover text - Maui dive width is 300 pixels and centered"){width="300" align="center"}
```

Gerenderd:

![Alternatieve tekst voor afbeelding duwen](assets/maui-dive.jpg "Tekst met aanwijzen - Maui-dive-breedte is 300 pixels en gecentreerd"){width="300" align="center"}

* Voor grote afbeeldingen raden we u aan afbeeldingen te maken die groot genoeg zijn om te worden verkleind tot de paginabreedte (ten minste 640 pixels breed). De aanbevolen breedte is 1500 pixels. U hoeft geen afbeeldingen te maken die groter zijn dan 2500 pixels of 500 kilobytes. De maximale bestandsgrootte voor afbeeldingen is 100 MB.
* Voor kleine afbeeldingen maakt u afbeeldingen met de gewenste breedte in pixels of gebruikt u de breedteparameter, zoals `{width="250"}` (pixels) of `{width="50%"}` (percentage van weergavegebied, niet de oorspronkelijke afbeeldingsgrootte). Afbeeldingen worden proportioneel geschaald. Houd er rekening mee dat afbeeldingen omhoog of omlaag kunnen worden geschaald, dus dat u voorzichtig moet zijn met pixelvorming.
* In sommige gevallen zien afbeeldingen van dezelfde interface er onevenredig uit op de pagina omdat bredere afbeeldingen (zoals een werkbalk) worden verkleind terwijl smalle afbeeldingen (zoals een deelvenster) niet worden verkleind. In dergelijke gevallen kunt u de bredere afbeeldingen verkleinen om de visuele consistentie te verbeteren.
* U kunt de uitlijning van een afbeelding wijzigen binnen het weergavegebied. Gebruik beide `{align="center"}` of `{align="right"}`. De `valign` parameter wordt niet ondersteund.

>[!NOTE]
>
De maximale bestandsgrootte voor afbeeldingen is 100 MB. Dat is de github.com-limiet. De limiet voor git.corp.adobe.com is hoger (250 MB), maar we moeten bestanden kunnen kopiëren naar de spiegel github.com.

### Afbeeldingskoppelingen

Als u wilt dat gebruikers op een afbeelding kunnen klikken om naar een andere pagina te gaan, gebruikt u deze indeling.

**Syntaxis**

```
[![image](assets/core-services_96.png)](https://www.adobe.com)
```

**Voorbeeld**

Klik op deze afbeelding om naar de website van de Adobe te gaan.

[![image](assets/core-services_96.png)](https://www.adobe.com)

<!--
### Click-to-zoom images

Use the `zoomable` parameter to allow users to click an image to view an enlarged version of the image. When the user mouses over a zoomable image, the pointer becomes a magnifying glass. When clicked, the image expands to the full width of the browser. It can be dismissed with a close button.

**Example**

![Diving image](/help/test-guide/assets/maui-dive.jpg "Diving in Maui"){width="100" zoomable="yes"}

**Syntax**

```
![Diving image](/help/test-guide/assets/maui-dive.jpg "Diving in Maui"){width="100" zoomable="yes"}
```

-->

## Koppelingen en kruisverwijzingen {#links-and-cross-references}

Externe koppelingen zijn recht-voorwaarts en kunnen worden weergegeven als een gekoppeld bijschrift of als een zuivere URL.

```
[Adobe](https://www.adobe.com)
```

Gerenderd:

[Adobe](https://www.adobe.com)

Als u een URL rechtstreeks aan tekst toevoegt, wordt deze niet automatisch omgezet in een koppeling. Als u een URL als koppeling wilt weergeven, voegt u `< >` syntaxis. Voorbeelden:

```
https://www.adobe.com

<https://www.adobe.com>
```

Gerenderd:

https://www.adobe.com

<https://www.adobe.com>

Koppelingen naar artikelen (kruisverwijzingen) kunnen iets complexer zijn.

**Optie 1: Standaard relatieve koppeling**

Zo ziet een standaard relatieve koppeling eruit:

```
See [Overview example article](collaborative-doc-instructions/overview.md)
```

De padnaam moet rekening houden met zowel de locatie van het bronbestand als het doelbestand. U kunt alle relatieve koppelingsoperanden gebruiken, zoals `./` (huidige map), `../` (één map terug), en `../../` (twee directory&#39;s terug).

**Optie 2: Relatieve hoofdkoppeling**

Het voordeel van dit type koppeling is dat alleen het doelbestand in de koppeling moet worden opgenomen. Het werkt vanuit elk bronbestand in de repo, ongeacht de locatie van het bronbestand.

```
/help/using/docile-rules/introduction.md
```

**Diepe koppeling**

Als u een koppeling wilt maken naar een kop in een artikel, moet de kop-id van het doel een expliciete kop bevatten (ook wel een &quot;anker-id&quot; genoemd). Voorbeeld:

`## Creating audience segments {#creating-audience-segments}`

Als u op dezelfde pagina een koppeling naar deze kop wilt maken, gebruikt u de kop-id als de koppeling:

`See [Creating audience segments](#creating-audience-segments)`

Als u vanuit een ander artikel in de repo een koppeling naar deze kop wilt maken, voegt u het achtervoegsel met de titel-id toe aan het einde van de koppeling:

`See [Audiences: Creating audience segments](audiences.md#creating-audience-segments)`

**Openen op nieuw tabblad**

Als u met een koppeling een nieuw tabblad wilt openen, bijvoorbeeld wanneer u naar een andere hulplijn gaat, gebruikt u de optie `{target="_blank"}` eigenschap in de koppeling.

Voorbeeld:

`[See What's new](whats-new.md){target="_blank"}`

## Metagegevens

Voeg metagegevens toe boven aan het markeringsbestand. De volgende regel na de metagegevensregel (en de lege regel) MOET de titel van het artikel (# Titel) zijn.

```
---
title: Title for search optimization
description: This is the article description used for search optimization. Use common search keywords and synonyms.
---

# Article title
```

## Lokalisatietags: UICONTROL, DNL en DONOTLOCALIZE

Al onze Help-inhoud voor Markdown is gelokaliseerd met behulp van in eerste instantie automatische vertaling. Als de hulp nooit is gelokaliseerd, dan houden wij de machinevertaling. Als de Help-inhoud echter in het verleden is gelokaliseerd, fungeert de door de computer vertaalde inhoud als plaatsaanduiding tijdens het vertalen van de inhoud.

## Meer als dit

Met de component ‘Meer als dit’ kunt u verwante koppelingen weergeven aan het einde van een artikel. Wanneer deze wordt gerenderd, wordt de component MORELIKETHIS gerenderd als &quot;Verwante artikelen&quot; (en gelokaliseerd in andere talen).

**Syntaxis**

![Meer als deze syntaxis](assets/morelikethis.png)

**Voorbeeld**

>[!MORELIKETHIS]
>
* [Artikel 1](https://helpx.adobe.com/nl/support/analytics.html)
* [Artikel 2](https://helpx.adobe.com/nl/support/audience-manager.html)

## Notities/correcties

We hebben Markering uitgebreid om verschillende typen notities op te maken: Opmerking, Tip, Belangrijk en Waarschuwing.

**Syntaxis**

```
>[!NOTE]
>
>This is a standard NOTE block.
```

**Voorbeeld**

>[!NOTE]
>
Dit is een standaardblok van de NOOT.

**Syntaxis**

```
>[!TIP]
>
>This is a standard tip.
```

**Voorbeeld**

>[!TIP]
>
Dit is een standaardtip.

**Syntaxis**

```
>[!WARNING]
>
>This is a standard warning block.
```

**Voorbeeld**

>[!WARNING]
>
Dit is een standaardwaarschuwingsblok.

**Syntaxis**

```
>[!IMPORTANT]
>
>This is a standard important block.
```

**Voorbeeld**

>[!IMPORTANT]
>
Dit is een belangrijk standaardblok.

**Syntaxis**

```
>[!NOTE]
>
>This is a standard NOTE block.
>
>It includes multiple paragraphs.
```

**Voorbeeld**

>[!NOTE]
>
Dit is een standaardblok van de NOOT.
>
Dit omvat meerdere alinea&#39;s.

Nieuwe ondersteunde typen notities:

>[!ADMIN]
>
Dit is een beheernotitie. Alleen EXL.

>[!AVAILABILITY]
>
Dit is een beschikbaarheidsnota. Alleen EXL.

>[!PREREQUISITES]
>
Dit is een notitie met voorwaarden. Alleen EXL.

>[!INFO]
>
Dit is een Info-notitie. Alleen EXL.

>[!ERROR]
>
Dit is een foutbericht. Alleen EXL.

>[!SUCCESS]
>
Dit is een succesopmerking. Alleen EXL.

## Genummerde lijsten en lijsten met opsommingstekens {#lists}

Als u genummerde lijsten wilt maken, begint u met een regel met `1.` of `1)`, maar kies één methode en gebruik deze consistent in het artikel. U hoeft de getallen niet op te geven. GitHub doet dat voor jou.

Het nummer gebruiken `1` voor elke stap in de genummerde lijst.

Voeg lege regels voor en na lijsten toe.

**Syntaxis**

```
1. This is step 1.

1. This is the next step.

   1. This is a sub-step

   1. This is a sub-step

1. This is yet another step, the third.
```

**Voorbeeld**

1. Dit is stap 1.

   1. Substap

   1. Substap

1. Dit is de volgende stap.

1. Dit is nog een stap, de derde.

Als u lijsten met opsommingstekens wilt maken, begint u met `*` of `-` of `+`, maar kies één methode en gebruik deze consistent in het artikel. (Als u de indelingen combineert, zoals `*` en `+`, krijgt u een de bevestigingsfout van de Prijsbevestiging wanneer u het dossier. incheckt)

**Beste praktijken:** Gebruiken `*` voor opsommingstekens. De Code van Visual Studio past de asterisk voor kogels toe, zodat is het gemakkelijker om met asterisken te blijven om het creëren van een ongeordende lijst te automatiseren. (U zou kunnen opgemerkt hebben dat het TOC.md- dossier plus ondertekenen gebruikt `+` voor lijsten. Dat is een holdover van migratie. Een geldig opsommingsteken werkt zolang het binnen het artikel consistent is.)

**Syntaxis**

```
* First item in an unordered list.
* Another item.
* Here we go again.
```

**Voorbeeld**

* Eerste item in een ongeordende lijst.
* Nog een item.
* Hier gaan we weer.

U kunt lijsten binnen lijsten ook insluiten en inhoud tussen lijstpunten toevoegen. Inspringen inhoud tussen lijstitems om te voorkomen dat een nieuwe lijst wordt gestart. Items tussen stappen moeten aan het begin van de tekst worden ingesprongen. Dit zijn drie spaties voor genummerde lijsten en twee spaties voor opsommingstekens.

```
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/core-services_96.png)
   
1. Make sure that your table looks like this: 

   | Hello | World |
   |---|---|
   | How | are you? |
   
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.
   
1. Do another step.

   This is an indented line.
```

**Voorbeeld**

1. Stel uw tabel- en codeblokken in.
1. Voer deze stap uit.

   ![scherm](assets/core-services_96.png)

1. Zorg ervoor dat uw tabel er zo uitziet:

   | Hallo | Wereld |
   |---|---|
   | Hoe | Ben je dat? |

1. Dit is de vierde stap.

   >[!NOTE]
   >
   Dit is notitietekst.

1. Doe nog een stap.

   Dit is een ingesprongen lijn.

NOTA: Als u te ver, zoals 6 ruimten in plaats van 3 inspringt, zal de inhoud in die lijn als een codeblok worden behandeld.

## Schaduwvakken

Schaduwvakken zijn handig om een inhoudssectie van de rest van de pagina in te stellen. Het Workfront-team voegt bijvoorbeeld graag &quot;Voorbeeld&quot;-vakken toe die tekst, afbeeldingen en codevoorbeelden bevatten voor een bepaald doel. Een schaduw kan ook handig zijn voor secties &#39;Op eigen&#39; of &#39;Hoofdletters gebruiken&#39; of voor uitgebreide notities of tips.

Als u een schaduwvak wilt maken, voegt u `>[!BEGINSHADEBOX]` aan het begin van de sectie en `>[!ENDSHADEBOX]` aan het einde. Alle inhoud tussen deze begin- en eindtags heeft een grijze achtergrond. Een label toevoegen aan `BEGINSHADEBOX` (zoals `>[!BEGINSHADEBOX "Use Case]` is een optionele manier om een titel van een bolvormig schaduw te maken. U kunt ook alleen vette tekst of een kop op de volgende regel plaatsen.

Voorbeeld:

>[!BEGINSHADEBOX]

**De rand in een HTML-tabel verwijderen**

In sommige gevallen gebruikt u een HTML-tabel om een evenwichtig ontwerp te maken, maar u wilt niet dat de inhoud eruit ziet als een tabel. Als u een rand wilt uitschakelen voor een HTML-tabel met één rij, gebruikt u de volgende syntaxis:

```
<table>
<tr style="border: 0;">
```

>[!NOTE]
>
Overmatig gebruik vermijden. Voor normale tabellen willen we een consistent ontwerp houden voor alle inhoud.

![tabeltip](assets/table-no-border.png)

In een tabel met drie kolommen kunt u ook `<td align="center">` en `<td align="right">` Hiermee verdeelt u de celinhoud gelijkmatig over het weergavegebied. Als dat niet het geval was, zou ik het u hebben gezegd.

Dit is de laatste regel van het schaduwvak.

>[!ENDSHADEBOX]

## Fragmenten en inclusief

Als u tekst wilt delen tussen artikelen in een repo, maakt u een `_includes` in de `help` map. Dit `_includes` map kan .md-bestanden bevatten waarnaar kan worden verwezen (opgenomen) vanuit andere bestanden in de repo. Bovendien `snippets.md` in dit repo-bestand kunnen ook Hoofd2-ankers zijn opgenomen waarnaar vanuit elk bestand in de repo kan worden verwezen.

Verwijzing naar H2 in snippets.md-bestand: `{{id-name}}`

Verwijzing naar include-bestand: `{{$include /help/_includes/filename.md}}`

## Tabellen

Tabellen kunnen problematisch zijn in Markering. Wanneer tabellen worden gemigreerd vanaf het vorige ontwerpsysteem, worden eenvoudige tabellen (één regel per cel) opgemaakt als native Markeringen (voorkeur). Geavanceerde tabellen worden opgemaakt als HTML.

>[!TIP]
>
Kijk naar de [Video over markeringstabellen](https://video.tv.adobe.com/v/26220)

Native tabellen zien er vaak beter uit in Markering. Kolommen worden geschaald op basis van hun inhoud. HTML-tabellen worden weergegeven met kolommen met gelijke breedte.

Standaard biedt Markdown geen ondersteuning voor meerdere regels of lijsten in cellen. Wij hebben echter de tabellen Markering uitgebreid om meerdere regels in cellen toe te staan (met `<p>` of `<br>`) of basislijsten (gebruiken `<ul><li>` enz.).

>[!IMPORTANT]
>
Wees voorzichtig wanneer u deze HTML-codes toevoegt aan Markeringen. Als uw syntaxis onjuist is, krijgt u een verwarrende validatiefout die het probleem niet nauwkeurig beschrijft. Controleer uw syntaxis van de HTML om ervoor te zorgen dat het behoorlijk-gevormd is.

Niet toegestaan in een tabel: iframes, reeksen cellen, ingesloten tabellen.

Niet toegestaan in de native vervolgkeuzelijst: geneste of complexe lijsten.

Zie [Tabellen](tables.md)

**Syntaxis**

```
| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | row 1 column 2 | row 1 column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

**Voorbeeld**

| Koptekst | Een andere header | Nog een kop |
|--- |--- |--- |
| rij 1 | rij 1 kolom 2 | rij 1 kolom 3 |
| rij 2 | rij 2 kolom 2 | rij 2 kolom 3 |

Eenvoudige tabellen werken naar behoren in Markering. Tabellen die meerdere alinea&#39;s of lijsten in een cel bevatten, zijn echter moeilijk te gebruiken. Voor dergelijke inhoud raden we u aan een andere indeling te gebruiken, zoals koppen en tekst.

**Markeringstabel met alinea-einden en lijsten**

```
| Header | Another header | Yet another header |
|------------|----------|----------------|
| row 1 | first paragraph in cell<p>second paragraph in cell(`<p>`)<br>line break (`br`) | row 1 column 3 |
| row 2 | bullet list<ul><li>item 1</li><li>item 2</li><li>item 3</li></ul> | row 2 column 3 |
```

**Voorbeeld**

| Koptekst | Een andere header | Nog een kop |
|------------|----------|----------------|
| rij 1 | eerste alinea in cel<p>tweede alinea in cel(`<p>`)<br>regeleinde (`br`) | rij 1 kolom 3 |
| rij 2 | lijst met opsommingstekens<ul><li>item 1</li><li>item 2</li><li>item 3</li></ul> | rij 2 kolom 3 |

**Markeringstabel met regeleinden en namaaklijst**

Oplossing met handmatige opsommingstekens.

```
| Color | Things to Do |
|--- |--- |
| Red | * Read <br> * Write <br> * Study |
| Blue | * Swim <br> * Run <br> * Lift <br> **Note**: Remember to train smart.|
```

**Voorbeeld**

| Kleur | Te doen dingen |
|--- |--- |
| Rood | * Lezen <br> * Schrijven <br> * Studie |
| Blauw | * Swim <br> * Uitvoeren <br> * Optillen <br> **Opmerking**: Vergeet niet slim te trainen. |
32


## Tabs

Een tab is een klikbaar gebied boven aan een sectie met verschillende inhoud. Wanneer op een tab wordt geklikt, wordt de inhoud van de tab weergegeven en wordt de inhoud van andere tabbladen verborgen.

Als u een tabset wilt maken, voegt u `>[!BEGINTABS]` aan het begin van de tabset en `>[!ENDTABS]` na de laatste tab. Toevoegen `>[!TAB <tab title>]` -tags voor elke tabsectie en voeg de inhoud van elk tabblad eronder toe.

**Tabsyntaxis**

```
>[!BEGINTABS]

>[!TAB iOS]

This content appears in the iOS tab.

>[!TAB Android]

This content appears in the Android tab.

>[!TAB Windows]

This content appears in the Windows tab.

>[!TAB MacOS]

This content appears in the MacOS tab.

>[!TAB Linux]

This content appears in the Linux tab.

>[!ENDTABS]
```

**Gerenderd**

>[!BEGINTABS]

>[!TAB iOS]

Deze inhoud wordt weergegeven op het tabblad iOS.

>[!TAB Android]

Deze inhoud wordt weergegeven op het tabblad Android.

>[!TAB Windows]

Deze inhoud wordt weergegeven op het tabblad Windows.

>[!TAB MacOS]

Deze inhoud wordt weergegeven op het tabblad MacOS.

>[!TAB Linux]

Deze inhoud wordt weergegeven op het tabblad Linux.

>[!ENDTABS]

**Tabnotities**

* Gebruikers kunnen zoeken in pagina&#39;s (Ctrl+F/Cmd+F) om inhoud te zoeken in tabbladen die niet worden weergegeven.
* Als de tabtitels de breedte van de paginaweergave in de browser van de gebruiker overschrijden, wordt een horizontale schuifbalk weergegeven.
* U kunt de tabtitels niet opmaken. Alle syntaxis die u toevoegt, wordt doorgegeven als onderdeel van de titel. Bijvoorbeeld: `>[!TAB **iOS**]` wordt weergegeven zoals `**iOS**`.
* U kunt meerdere tabsets op een pagina maken, maar u kunt een tabset niet nesten binnen een andere tabset.
* Er wordt een gearceerde achtergrond toegepast op de tabset, zodat gebruikers de tabinhoud kunnen onderscheiden van andere inhoud.

## Tekstmarkering

Het Workfront-team heeft gevraagd gele markering te kunnen gebruiken om de voorvertoning van aanstaande functies aan te geven. Zo werkt het.

Voorbeeld:

```
This entire paragraph should NOT be highlighted. <span class="preview"> This word is **bold** inside a highlighted sentence.</span> And this is just the last sentence.
```

Gerenderd:

Deze hele alinea mag NIET worden gemarkeerd. <span class="preview"> Dit woord is **vet** in een gemarkeerde zin.</span> Dit is slechts de laatste zin.

Als algemene regel geldt dat `<span class="preview">` om een alinea of tekst in een alinea te markeren en te gebruiken `<div class="preview">` voor meerdere alinea&#39;s en componenten.

>[!NOTE]
>
We zijn nog steeds bezig de markeerweergave van bepaalde pagina-elementen, zoals notities en tabellen, te verbeteren. Voel u vrij om JIRA-bugs te registreren als u onjuiste rendering ziet. In uitvoering.
>
VSC-voorvertoning biedt nog geen ondersteuning voor markering.

## Video

Video&#39;s worden niet native gerenderd in Markdown. Gebruik de componentindicator om een video inline weer te geven `[!VIDEO]` en dan de url.

**Syntaxis**

```
>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)
```

**Voorbeeld**

>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)

## Aanvullende syntaxisgegevens voor markeringen

### Uitgebreide opmaakcomponenten

We moeten Markering uitbreiden om items te ondersteunen die niet zijn opgenomen in gemeenschappelijke markeringen.

Speciale componenten worden gedeclareerd in een bevattende blokaanhaling met behulp van vierkante haken en een uitroepteken plus de referentie voor het type blok dat het is. Hier ziet u bijvoorbeeld hoe u een notitie declareert:

```
>[!NOTE]
>
>This is a note.
```

* Notities (aanbevelingen), waaronder Notitie, Belangrijk, Tip, Let en Waarschuwing
* Ingesloten video
* Meer als dit (verwante artikelen)
* Verschillende UI-tags voor lokalisatie
* Componenteigenschappen voor koppen, afbeeldingen en codeblokken
* Inklapbare secties
* Tekstmarkering
* Tabbladen Pagina

Het blokcitaat van de Markering gebruiken ( `>` ) aan het begin van elke regel om een op alinea&#39;s gebaseerde component, zoals een opmerking, samen te voegen. Als u de voorvertoning wilt verbeteren, voegt u direct na het begin van de sectie een regel toe die alleen een blokaanhalingsteken bevat (`>`). Voeg een lege regel toe om de sectie te beëindigen.

Als u subcomponenten binnen componenten moet gebruiken, voegt u een extra niveau van blokcitaten toe (`>  >`) voor die onderdeelsectie. Bijvoorbeeld, zou een NOTA binnen een sectie DONOTLOCALIZE met moeten beginnen `>  >`.

In sommige gevallen moeten we specifieke instellingen voor opmaakelementen, zoals koppen, ondersteunen. Als u de standaardinstellingen moet wijzigen, voegt u de parameters tussen de franse accolades toe `{# }` na de component.

### Lege lijnen

U kunt wat ademruimte toevoegen aan uw wanden van tekst met lege lijnen. Gebruiken `<br>&nbsp;` als tijdelijke oplossing om een lege regel toe te voegen.

Voorbeeld: dit is een eerste zin van wat een heel lange tekst zou kunnen zijn. Laat mij een lege regel tussen deze paragraaf en de volgende toevoegen.

<br> 

Dit lijkt hier misschien niet erg indrukwekkend, maar probeer blanco regels uit als je je pagina&#39;s te vol vindt.

### Te &#39;escape&#39;-tekens {#characters-to-escape}

Verschillende tekens (`# { } [ ] < > * + - . !`) hebben een speciale betekenis in Markeringen of HTML voor het maken van koppen, afbeeldingen, lijsten en andere componenten. Wanneer u deze tekens gebruikt, denkt de renderingengine dat u code toevoegt. In sommige gevallen wilt u deze tekens echter wel in uw tekst weergeven. Om dat te doen, moet je de karakters &quot;ontsnappen&quot;. De eenvoudigste manier om te ontsnappen is om het teken voor te gaan met een backslash (`\`). Als u bijvoorbeeld een regel wilt beginnen met een `#` teken zodat het niet als een kop wordt geïnterpreteerd, zou u typen `\#`:

`\# This is not a heading`

**Gerenderd:**

\## Dit is geen kop

De backslash werkt alleen met de volgende tekens: `# { } [ ] * + - . !`. Als u tekens zoals punthaakjes moet laten ontsnappen (zoals `<yourname>`), kunt u of de tekst in achtertikken insluiten om een gealigneerd codeblok toe te passen, of de HTML entiteitcode in plaats van het karakter gebruiken. Voorbeelden van algemene HTML-codes:

* `&lt;` (&lt;)
* `&gt;` (>)
* `&amp;` (&amp;)
* `&Hat;` (^)
* `&mdash;` (—)
* `&ndash;` (-)

Een volledige lijst met HTML-entiteiten is beschikbaar op de [Freeformatter-website](https://www.freeformatter.com/html-entities.html). Hierdoor kunt u alle speciale tekens opzoeken.

>[!NOTE]
>
Voor kettingstappen zoals &quot;Kies Bestand > Opslaan als&quot; hoeft u de opdracht `>` teken omdat het niet naast andere tekens staat. Voor variabelen zoals `<filename>` u zult de punthaken willen ontsnappen gebruikend één van beide codeblok `backticks` of tekencodes (`&lt;filename&gt;`).

Als u HTML-entiteiten in codeblokken gebruikt, wordt de eenheidstekst niet omgezet in het speciale teken. Bijvoorbeeld: `&gt;` verschijnt in een codeblok als &quot; `&gt;` &quot; in plaats van &quot; > &quot;.

Om achtertikken (&grave; ) te ontsnappen, gebruik `&grave;` of plaats de achterste tik binnen drievoudige achtertikken die een gealigneerd codeblok verpakken.

### Niet-ondersteunde items

Er zijn een paar Git-gearomatiseerde Markeringen die we niet willen ondersteunen. Het voorvertoningsgereedschap dat u gebruikt, schakelt sommige van deze functies mogelijk in, maar vertrouwt erop.

**Taaklijst**

Niet ondersteund

```
* [x] Set up Jersey Shore recording
* [x] Buy donuts with sprinkles
* [x] Take nap
* [ ] Wash ferret
```

**Emoji**

Niet ondersteund

```
:bowtie:
```

**Horizontale lijn**

Niet ondersteund

```
***
```

**Aanhalingstekens blokkeren**

We gebruiken blokaanhalingstekens (`>` aan het begin van een regel) naar de aangegeven uitgebreide syntaxis voor markeringen, zoals notities en video&#39;s, zoals hieronder wordt beschreven. Maar u kunt ook `>` syntaxis om een blokaanhalingssectie te maken.

>[!NOTE]
>
Als u te ver inspringt, zoals zes spaties in plaats van drie, wordt de inhoud weergegeven als blokaanhalingstekens. Gebruik de juiste hoeveelheid inspringing om te voorkomen dat de inhoud per ongeluk wordt weergegeven als een blokaanhalingsteken.
