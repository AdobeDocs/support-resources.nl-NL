---
title: Bugfixes (verborgen)
description: Testpagina voor interne testdoeleinden
hide: true
hidefromtoc: true
exl-id: e6270f95-3550-4e35-ad4c-760584bb9b5d
source-git-commit: 0cefcf5bb4a021593a6bbe44eed0ad83e8bd259f
workflow-type: tm+mt
source-wordcount: '1926'
ht-degree: 23%

---

# Bugfixes

## Autoactiveringstest

Deze bugs moeten allemaal worden opgelost.

## UGP-10866 Koppelingen niet vet in schaduwvakken

>[!BEGINSHADEBOX]

**Lijst van inhoud**

* [Aan de slag met de AI Assistant](note-test.md)
* **[E-mailgeneratie met de Medewerker AI](syntax-style-guide.md)**
* [SMS genereren met de AI Assistant](test-page.md)
* [Push generation met de AI Assistant](tables.md)
* [Inhoud experimenteren met de AI Assistant](test-redirection.md)

>[!ENDSHADEBOX]

Geen schaduw

**Lijst van inhoud**

* [Aan de slag met de AI Assistant](note-test.md)
* **[E-mailgeneratie met de Medewerker AI](syntax-style-guide.md)**
* [SMS genereren met de AI Assistant](test-page.md)
* [Push generation met de AI Assistant](tables.md)
* [Inhoud experimenteren met de AI Assistant](test-redirection.md)


## UGP-10584 Inlinebadges werken niet

Deze badges moeten op dezelfde regel staan als de opsommingstekens.

* [[!DNL Mixpanel]](note-test.md) [!BADGE &#x200B; Nota&#39;s &#x200B;]{type=Informative}
* [[!DNL Pendo]](tables.md) [!BADGE &#x200B; Lijsten &#x200B;]{type=Positive}
* [[!DNL RainFocus]](syntax-style-guide.md) [!BADGE &#x200B; Gids van de Stijl van de Syntaxis &#x200B;]{type=Positive}

## UGP-10560 - Badges in inklapbare gedeelten

+++ Vorige versies

### V1.16 Release

_feb 13, 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ de Nieuwe ](assets/package.png) video&#39;s van het Product worden nu gesteund door de Dienst API van de Catalogus.
 de producten van de Reparatie van 0&rbrace; &lbrace;met vaste prijzen worden nu gesteund.
![&#128279;](assets/package.png)
![&#128279;](assets/package.png) de uit-van-voorraad opties van 0&rbrace; herstellen &lbrace;worden nu getoond in PDP widget.

#### Bekende beperkingen

Deze functies worden nog niet ondersteund:

* Maximale grootte voor dynamische attributen lading is 9 MB.
* Productprijs per groep. Kan worden berekend met eenvoudige productprijzen.
* In een afbeeldingsarray bevat alleen de eerste afbeelding rollen.

De volgende beperkingen kunnen worden opgelost met behulp van het API-net en de Core GraphQL API:

* Minimale geadverteerde prijs
* [ Rij tarifering ](https://www.adobe.com)

### V1.13 Release

_vrijdag 12 oktober 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Dienst van de Catalogus steunt de `inStock` vlag voor productvarianten.
![ Nieuw ](assets/package.png) `urlKey` en `externalId` zijn toegevoegd aan het schema van GraphQL.
![ Nieuwe ](assets/package.png) Downloadbare producten en geschenkkaarten worden nu gesteund.

### V1.12 Release

_woensdag 19 september 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](https://www.adobe.com).
![ Repareren ](assets/package.png) Deze versie bevat insectenmoeilijke situaties en verbeteringen op de de dienstkant.

### V1.11 Release

_woensdag 18 juli 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Dienst van de Catalogus steunt nu de [`recommendations` ](https://developer.adobe.com/commerce/services/graphql/recommendations/recommendations/) vraag van GraphQL voor Product Recommendations.

### V1.10 Release

_woensdag 27 juni 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) API van de Dienst van de Catalogus steunt nu &quot;verwante producten&quot;.

### V1.7-release

_donderdag 12 april 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Dienst van de Catalogus ontruimt nu geschrapte productvarianten.
![ verbeter ](assets/package.png) scalability van de Infrastructuur en prestatiesverbeteringen.

### V1.6-release

_woensdag 28 maart 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Toegevoegde stalen aan de [`products` ](https://developer.adobe.com/commerce/services/graphql/catalog-service/products/) vraag.
![ Nieuw ](https://www.adobe.com).

### V1.5-release

_dinsdag 6 maart 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Toegevoegde [`categories` ](https://developer.adobe.com/commerce/services/graphql/schema/catalog-service/categories/) functionaliteit van GraphQL.
![ verbeter ](assets/package.png) Verbeterde prestaties en API scalability.

### V1.4 Release

_woensdag 7 februari 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Gepubliceerde catalogus-dienst metapakket om installatiestappen te vereenvoudigen.
![ bevestig ](assets/package.png) API scalability en prestatiesverbeteringen.

### V1.3 Release

_woensdag 17 januari 2023_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](assets/package.png) Vereenvoudigde en verbeterde de onboarding ervaring.
![ Nieuwe ](assets/package.png) de nieuwe eindpunten van de klantenzandbak zijn beschikbaar voor preproductie het testen.
![ Nieuwe ](assets/package.png) Steun die voor virtuele producten wordt toegevoegd.
![ bevestig ](assets/package.png) API scalability en prestatiesverbeteringen.

### V1.1-release

_zaterdag 18 november 2022_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Dienst van de Catalogus steunt nu het 2&rbrace; API Net van de Adobe .
[&#128279;](https://developer.adobe.com/graphql-mesh-gateway/?lang=nl)
![ bevestig ](assets/package.png) Verbeterde API scalability en algemene prestaties.

### V1.0-release

_woensdag 4 oktober 2022_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) steun nu gebundelde en gegroepeerde producten.
![ Nieuwe ](assets/package.png) Toegevoegde B2B zichtoverschrijvingen. De producten zijn nu doorzoekbaar en kunnen aan de kar voor specifieke klantengroepen worden toegevoegd.
![&#128279;](assets/package.png) de Dienst van 0&rbrace; Repareren &lbrace;is nu stabieler en heeft betere prestaties.

### 0.3 Release - Beta+

_dinsdag 12 september 2022_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuwe ](assets/package.png) Beelden voor variantsteun: de productbeelden zijn teruggekeerd gebaseerd op de geselecteerde opties
![ Nieuwe ](assets/package.png) Rollen voor prijssteun: sta slechts leden van specifieke klantengroepen toe om de prijs van producten te zien
![ bevestig ](assets/package.png) Verbeterde stabiliteit en prestaties van de dienst
![ Nieuwe ](assets/package.png) Updates worden ontvangen wanneer de producten van de catalogus worden geschrapt

### Beta Release

_woensdag 9 augustus 2022_

[!BADGE &#x200B; Gesteund &#x200B;]{type=Informative tooltip="Ondersteund"}

![ Nieuw ](assets/package.png) de vragen `products` en `refineProduct` keren de volgende gegevens terug:

* Vooraf gedefinieerde (systeem)productkenmerken.
* Dynamische productkenmerken en filter deze op rol (pagina met productweergave/productlijst).
* Productopties.
* Productafbeeldingen en filteren op rol (PDP/PLP).
* Een specifieke prijs voor eenvoudige producten en prijsbereiken voor configureerbare producten.
* Prijzen en prijsbereiken van de klantengroep. Ze retourneren een fallback-standaardprijs voor kopers zonder een klantengroep.
* Producttypen die gebruikmaken van klantspecifieke B2B-prijzen.

+++

## [!BADGE Afgeschaft]{type=negative}

Zie bovenstaande kop. En de volgende.

## Testen op automatisch activeren

Ik voegde dit toe op vrijdagmiddag maar klik niet op Publish Now.

### [!BADGE Bèta]{type=Informative}

Bob

## UGP-10565 - Tekst markeren

Tekst voor `<div class="preview">`

<div class="preview">

### Native Workfront-velden toevoegen

U kunt eigen Workfront-velden toevoegen aan uw aangepaste formulieren. Wanneer het aangepaste formulier aan een object is gekoppeld, wordt het veld gevuld met de objectgegevens. Het veld Beschrijving op een aangepast formulier dat aan een project is gekoppeld, wordt bijvoorbeeld toegevoegd aan de projectbeschrijving. (Het veld mag &quot;N.v.t.&quot; weergeven als er geen gegevens beschikbaar zijn.)

1. Op de linkerkant van het scherm, vind **Inheems gebied** en sleep het aan een sectie op het canvas.
1. Configureer rechts in het scherm de opties voor het aangepaste veld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven het veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b> BELANGRIJK </b>: Gebruik geen speciale karakters in dit etiket. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam geeft het systeem het veld aan.</p><p> Wanneer u het veld voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p>
      <p><b> BELANGRIJK </b>:
      <ul> 
      <li>Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in Workfront hebben gebruikt. Als u dat doet, herkent het systeem niet langer het veld waar er nu naar kan worden verwezen in andere gebieden van Workfront.</p> </li>
      <li> <p>Elke veldnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt.</p> </li>
      <li><p>We raden u aan het teken punt/punt niet te gebruiken in de aangepaste veldnaam om fouten te voorkomen bij het gebruik van het veld in verschillende gebieden van Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>Typ eventuele aanvullende informatie over het veld. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Referentieveld</td> 
      <td><p>(Vereist) Selecteer een eigen Workfront-veld.<p><p>Alleen native velden voor de objecten van het formulier zijn beschikbaar. Als bijvoorbeeld de lijst Objecttypen boven aan de formulierontwerper Project weergeeft, kunt u native velden selecteren voor projecten, maar niet voor velden die specifiek zijn voor taken.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Grootte</td> 
      <td>(Optioneel) Wijzig desgewenst de weergavegrootte van het veld.</td> 
     </tr> 
    </tbody> 
   </table>

1. Om uw veranderingen te bewaren, **van toepassing is** en zich op een andere sectie te bewegen om uw vorm verder te bouwen.

   of

   Klik **sparen en Sluiten**.

</div>

Tekst na markering

## UGP-10566 - De tekst van de verbinding is kleiner dan regelmatige tekst in HTML lijsten

Zie ook UGP-9780

<table style="table-layout:auto"> 
<tbody> 
<tr>
<td>Invoer naar</td>
<td>Beschrijving</td>
<td>Beschikbaar voor </td>
</tr>
<tr> 
    <td role="rowheader">Label</td> 
    <td> <p>(Vereist) Typ een beschrijvend label dat boven het aangepaste veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen. Voor meer informatie, zie <a href="https://www.adobe.com" class="MCXref xref"> een douanegebied aan een douanevorm </a> in dit artikel toevoegen.</p> <p><b> BELANGRIJK </b>: Gebruik geen speciale karakters in dit etiket. Ze worden niet correct weergegeven in rapporten.</p> </td> 
    <td>
    <ul>
    <li>Keuzerondjes. Voor meer informatie, zie <a href="https://www.adobe.com"> een douanegebied aan een douanevorm </a> in dit artikel toevoegen. (Geen klasse)</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
</tr> 
</tbody> 
</table>

## UGP-9176 - Oude bug

De tag &quot;span&quot; werkt niet goed in een notitie (en lijst)

Voor informatie over welke eigenschappen in de nieuwe het becommentariëren ervaring en voor welke voorwerpen beschikbaar zijn, zie [ Nieuwe het becommentariëren ervaring ](note-test.md).

1. Ga naar het object waaraan u een antwoord wilt toevoegen.
1. Klik **Updates**, dan klik het **3&rbrace; lusje van Commentaren &lbrace;voor het voorwerp en vind de commentaar of het antwoord waarop u wilt antwoorden**

   of

   <span class="preview"> klik het **Al** lusje, dan klik **Antwoord in Commentaren** om de opmerking in het lusje van Commentaren te openen en aan het te antwoorden. U kunt niet op het Al lusje antwoorden.</span>

1. (Facultatief) om tekst van een vorige update in uw antwoord te omvatten, klik het **Meer** menu in de hoger-juiste hoek van de commentaar u wilt antwoorden aan, dan **antwoord van het Citaat** klikken. De tekst van de vorige update wordt weergegeven in het invoergebied, gemarkeerd met een verticale grijze lijn.
1. Klik **Reageren**.

   ![](assets/package.png)

   U kunt de gebruikers zien die actief in het gesprek bij de bodem van **betrokken zijn voeg antwoord toe..** doos en u kunt meer toevoegen, of degenen verwijderen die niet meer relevant zijn. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord. U kunt ook tags toewijzen aan meer gebruikers om deze in uw antwoord op te nemen.  Om meer gebruikers te etiketteren, zie [ Tags anderen op updates ](note-test.md).

   >[!TIP]
   >
   >   Om extra antwoorden aan een bestaand antwoord toe te voegen, kunt u beginnen in **te typen toevoegt antwoord...** doos, of **antwoordt** op de originele commentaar. Uw antwoord wordt toegevoegd aan het eind van de draad.

1. Begin uw antwoord te typen en gebruik om het even welke extra opties van de Rich toolbar van de Tekst. Voor informatie over het gebruiken van Rijke Tekst of andere het bijwerken mogelijkheden, zie [ het werk van de Update ](note-test.md).

1. Klik **voorleggen** om het antwoord te bewaren.

1. (Facultatief) klik het **Meer** menu in de hoger-juiste hoek van de commentaar u voor meer opties wilt antwoorden om het antwoord te beheren. Voor meer informatie, zie [ het werk van de Update ](note-test.md).


## UGP-10614 - Probleemtabellen met afbeeldingen

Ik denk dat de parameter `{width="20"}` problemen in tabellen veroorzaakt.

## Vergelijking van Success-lidmaatschappen voor Expert en Ultimate

|  | Success-lidmaatschap voor Expert | Ultimate Success-lidmaatschap |
|--- |--- |--- |
|  | Met het Expert Success-lidmaatschap hebt u toegang tot **24x7 deskundige ondersteuning** voor technische probleemoplossing en begeleiding bij uw kritieke bedrijfsproblemen. Of u kunt snelle oplossingen vinden door gebruik te maken van onze zelfstudiebronnen, exclusieve best practices en een online community van Adobe-experts en collega&#39;s. <p> *Bij alle Adobe Experience Cloud-licenties inbegrepen.* | Met het Ultimate Success-lidmaatschap krijgt u **strategische begeleiding en proactieve technische status om goed presterende digitale ervaringen te leveren**. Uw Adobe-omgeving wordt ondersteund door een team van experts die bekend zijn met uw bedrijf en gericht zijn op het uitvoeren van een roadmap die is afgestemd op uw doelstellingen en prioriteiten voor zakelijke impact. |
| **Succesteam** | Samengesteld team van ondersteuningstechnici | Omvat: <ul><li> Aangewezen Technische accountmanager </li><li> Aangewezen Customer Success Manager </li><li> Aangewezen Support Services Manager</li><li> Samengesteld team van technische specialisten en strategische deskundigen die Succes Accelerators leveren </li><li> Samengesteld team van ondersteuningstechnici </li></ul> |
| **Proactieve technische en operationele ondersteuning** | ![niet inbegrepen pictogram](../assets/Cross_red_circle.svg){width="20"} Niet inbegrepen | Omvat: <ul><li>Revisies voor upgrades en migratie, voorbereiding van release </li><li>Evaluaties van productroadmaps</li><li> Afgestemde technische en strategische roadmaps</li><li>Voorbereiding en planning van belangrijke gebeurtenissen</li><li>Planning voor relevante en tijdige activering</li><li>Technische best practices en sectorbegeleiding</li><li>Adviseren/afstemmen met productteams</li><li>Een uniform plan om de belangrijkste bedrijfsdoelstellingen te bereiken - Wederzijds actieplan (MAP)</li></ul> |
| **Technische ondersteuning** | Omvat: <ul><li>**P1**: 24x7 probleemondersteuning</li><li>**P2, P3, P4**: ondersteuning tijdens kantooruren</li><li>Beheer van standaard storingen</li><li>Samengesteld escalatiebeheer</li></ul> | Omvat: <ul><li>**P1**: 24x7 probleemondersteuning</li><li>**P2/P3**: 24x5-ondersteuning bij problemen</li><li>**P4**: ondersteuning tijdens kantooruren</li><li>Prioriteit gegeven aan het beheer van storingen</li><li>Aangewezen deskundig escalatiebeheer</li></ul> |
| **Success Accelerators** | ![niet inbegrepen pictogram](../assets/Cross_red_circle.svg){width="20"} Niet inbegrepen | Success Accelerators die regelmatig door TAM en CSM worden gepland<p>*(zie Success Accelerator-catalogus voor meer informatie)* |
| **Ondersteuningskanalen** | Online, telefoon, Experience League, forums | Gepersonaliseerd online portal, telefoon met prioriteit, Experience League, forums |

{style="table-layout:fixed"}

## Add-ons voor ondersteuning

| Add-ons | Success-lidmaatschap voor Expert | Ultimate Success-lidmaatschap |
|--- |--- |--- |
| **Add-on voor gebeurtenisbeheer**<br>: biedt end-to-end leiderschap en ondersteuning die nodig zijn om de gehele levenscyclus van belangrijke gebeurtenissen te beheren | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Add-on voor Technical Account Director**<br> Uw belangrijkste technische resource die toezicht houdt op het leiderschap, eigenaar is van de betrokkenheid van managers en zorgt voor governance om uw bedrijfsresultaten te maximaliseren | ![niet beschikbaar pictogram](../assets/Cross_red_circle.svg){width="20"} Niet beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Geavanceerde add-on voor cloudondersteuning**<br> Topzorg en waardegarantie voor klanten van Adobe Experience Manager as a Cloud Service | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Add-on voor mentorsessies**<br> Biedt op vaardigheden gebaseerd leren via een just-in-time trainingsmethode | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |
| **Add-on voor Developer Boost**<br> Dit verleent toegang tot de technische experts die met herstelwerk kunnen helpen | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![inbegrepen pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |
| **Add-on voor Prioriteitswachtrijbundel**<br> Sla de wachtrij over, zodat uw tickets het eerst worden behandeld met extra toegang tot mentorsessies en Developer Boost | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![inbegrepen pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |

{style="table-layout:fixed"}
