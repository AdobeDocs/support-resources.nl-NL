---
title: Bugfixes (verborgen)
description: Testpagina voor interne testdoeleinden
hide: true
hidefromtoc: true
source-git-commit: c31246781e212041bf0555cd2db71c4d0c555410
workflow-type: tm+mt
source-wordcount: '1827'
ht-degree: 1%

---

# Bugfixes

## UGP-10584 Inlinebadges werken niet

Deze badges moeten op dezelfde regel staan als de opsommingstekens.

* [[!DNL Mixpanel]](note-test.md) [!BADGE Notities]{type=Informative}
* [[!DNL Pendo]](tables.md) [!BADGE Tabellen]{type=Positive}
* [[!DNL RainFocus]](syntax-style-guide.md) [!BADGE Handleiding voor syntaxisstijl]{type=Positive}

## UGP-10560 - Badges in inklapbare gedeelten

+++ Vorige versies

### V1.16 Release

_13 feb. 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Productvideo&#39;s worden nu ondersteund door de API voor catalogusservice.
![Repareren](assets/package.png) Er wordt nu steun verleend voor bundelproducten met vaste prijzen.
![Repareren](assets/package.png) Opties buiten de voorraad worden nu weergegeven in de PDP-widget.

#### Bekende beperkingen

Deze functies worden nog niet ondersteund:

* Maximale grootte voor dynamische attributen lading is 9 MB.
* Productprijs per groep. Kan worden berekend met eenvoudige productprijzen.
* In een afbeeldingsarray bevat alleen de eerste afbeelding rollen.

De volgende beperkingen kunnen worden opgelost met behulp van het API-net en de Core GraphQL API:

* Minimale geadverteerde prijs
* [Tier-prijsstelling](https://www.adobe.com)

### V1.13 Release

_vrijdag 12 oktober 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Catalogusservice ondersteunt de `inStock` markering voor productvarianten.
![Nieuw](assets/package.png) `urlKey` en `externalId` zijn toegevoegd aan het GraphQL-schema.
![Nieuw](assets/package.png) Downloadbare producten en cadeaukaarten worden nu ondersteund.

### V1.12 Release

_woensdag 19 september 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](https://www.adobe.com).
![Repareren](assets/package.png) Deze versie bevat insectenmoeilijke situaties en verbeteringen aan de de dienstkant.

### V1.11 Release

_woensdag 18 juli 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Catalogusservice biedt nu ondersteuning voor de [`recommendations`](https://developer.adobe.com/commerce/services/graphql/recommendations/recommendations/) GraphQL-query voor Product Recommendations.

### V1.10 Release

_woensdag 27 juni 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) De API voor catalogusservice ondersteunt nu &quot;verwante producten&quot;.

### V1.7-release

_donderdag 12 april 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) De Catalogusservice schoont verwijderde productvarianten op.
![Repareren](assets/package.png) Verbeterde schaalbaarheid en prestaties van de infrastructuur.

### V1.6-release

_woensdag 28 maart 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Stalen toegevoegd aan de [`products`](https://developer.adobe.com/commerce/services/graphql/catalog-service/products/) query.
![Nieuw](https://www.adobe.com).

### V1.5-release

_dinsdag 6 maart 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Toegevoegd [`categories`](https://developer.adobe.com/commerce/services/graphql/schema/catalog-service/categories/) GraphQL-functionaliteit
![Repareren](assets/package.png) Verbeterde prestaties en API-schaalbaarheid.

### V1.4 Release

_woensdag 7 februari 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Gepubliceerde metapakket voor catalogusservices om installatiestappen te vereenvoudigen.
![Repareren](assets/package.png) Schaalbaarheid van API&#39;s en prestatieverbeteringen.

### V1.3 Release

_woensdag 17 januari 2023_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Vereenvoudigde en verbeterde ervaring bij het instappen.
![Nieuw](assets/package.png) Er zijn nieuwe eindpunten van de sandbox van de klant beschikbaar voor preproductietests.
![Nieuw](assets/package.png) Ondersteuning toegevoegd voor virtuele producten.
![Repareren](assets/package.png) Schaalbaarheid van API&#39;s en prestatieverbeteringen.

### V1.1-release

_zaterdag 18 november 2022_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Catalogusservice biedt nu ondersteuning voor de Adobe [API-net](https://developer.adobe.com/graphql-mesh-gateway/).
![Repareren](assets/package.png) Verbeterde API-schaalbaarheid en algemene prestaties.

### V1.0-release

_woensdag 4 oktober 2022_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Ondersteuning voor gebundelde en gegroepeerde producten.
![Nieuw](assets/package.png) Extra B2B-zichtbaarheidsoverschrijvingen. De producten zijn nu doorzoekbaar en kunnen aan de kar voor specifieke klantengroepen worden toegevoegd.
![Repareren](assets/package.png) De service is nu stabieler en de prestaties zijn verbeterd.

### 0.3 Release - bèta+

_dinsdag 12 september 2022_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) Afbeeldingen voor ondersteuning door varianten: productafbeeldingen worden geretourneerd op basis van de geselecteerde opties
![Nieuw](assets/package.png) Rollen voor prijsondersteuning: alleen leden van specifieke klantengroepen de prijs van producten laten zien
![Repareren](assets/package.png) Verbeterde stabiliteit en prestaties van de dienst
![Nieuw](assets/package.png) Updates worden ontvangen wanneer producten uit de catalogus worden verwijderd

### Bètaversie

_woensdag 9 augustus 2022_

[!BADGE Ondersteund]{type=Informative tooltip="Ondersteund"}

![Nieuw](assets/package.png) De `products` en `refineProduct` query&#39;s retourneren de volgende gegevens:

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

### [!BADGE Beta]{type=Informative}

Bob

## UGP-10565 - Tekst markeren

Tekst voor `<div class="preview">`

<div class="preview">

### Native Workfront-velden toevoegen

U kunt eigen Workfront-velden toevoegen aan uw aangepaste formulieren. Wanneer het aangepaste formulier aan een object is gekoppeld, wordt het veld gevuld met de objectgegevens. Het veld Beschrijving op een aangepast formulier dat aan een project is gekoppeld, wordt bijvoorbeeld toegevoegd aan de projectbeschrijving. (Het veld mag &quot;N.v.t.&quot; weergeven als er geen gegevens beschikbaar zijn.)

1. Op de linkerkant van het scherm, vind **Oorspronkelijk veld** en sleep het naar een sectie op het canvas.
1. Configureer rechts in het scherm de opties voor het aangepaste veld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven het veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam geeft het systeem het veld aan.</p><p> Wanneer u het veld voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p>
      <p><b>BELANGRIJK</b>:
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

1. Als u de wijzigingen wilt opslaan, klikt u op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

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
    <td> <p>(Vereist) Typ een beschrijvend label dat boven het aangepaste veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen. Zie voor meer informatie <a href="https://www.adobe.com" class="MCXref xref">Een aangepast veld toevoegen aan een aangepast formulier</a> in dit artikel.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
    <td>
    <ul>
    <li>Keuzerondjes. Zie voor meer informatie <a href="https://www.adobe.com">Een aangepast veld toevoegen aan een aangepast formulier</a> in dit artikel. (Geen klasse)</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
</tr> 
</tbody> 
</table>

## UGP-9176 - Oude bug

De tag &quot;span&quot; werkt niet goed in een notitie (en lijst)

Ga voor meer informatie over de functies die beschikbaar zijn in de nieuwe opmerkingervaring en voor welke objecten [Nieuwe ervaring met opmerkingen](note-test.md).

1. Ga naar het object waaraan u een antwoord wilt toevoegen.
1. Klikken **Updates** en klik vervolgens op de knop **Opmerkingen** tabblad voor het object en zoek naar de opmerking of het antwoord waarop u wilt reageren

   of

   <span class="preview">Klik op de knop **Alles** tab, en klik vervolgens op **Reageren in opmerkingen** om de opmerking te openen op het tabblad Opmerkingen en erop te reageren. U kunt niet reageren op het tabblad Alles.</span>

1. (Optioneel) Als u tekst uit een vorige update wilt opnemen in uw antwoord, klikt u op de knop **Meer** in de rechterbovenhoek van de opmerking waarop u wilt reageren, klikt u op **Offerteantwoord**. De tekst van de vorige update wordt weergegeven in het invoergebied, gemarkeerd met een verticale grijze lijn.
1. Klikken **Antwoord**.

   ![](assets/package.png)

   U kunt de gebruikers zien die actief in het gesprek bij de bodem van zijn betrokken **Antwoord toevoegen...** en kunt u meer toevoegen of verwijderen van de niet-relevante vakken. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord. U kunt ook tags toewijzen aan meer gebruikers om deze in uw antwoord op te nemen.  Als u meer gebruikers wilt labelen, raadpleegt u [Andere tags toepassen op updates](note-test.md).

   >[!TIP]
   >
   >   Als u aanvullende antwoorden op een bestaande reactie wilt toevoegen, kunt u beginnen met typen in het dialoogvenster **Antwoord toevoegen...** of klik op **Antwoord** op de oorspronkelijke opmerking. Uw antwoord wordt toegevoegd aan het eind van de draad.

1. Begin uw antwoord te typen en gebruik om het even welke extra opties van de Rich toolbar van de Tekst. Voor informatie over het gebruiken van RTF of andere het bijwerken mogelijkheden, zie [Werk bijwerken](note-test.md).

1. Klikken **Verzenden** om het antwoord op te slaan.

1. (Optioneel) Klik op de knop **Meer** in de rechterbovenhoek van de opmerking waarop u wilt reageren voor meer opties voor het beheren van de reactie. Zie voor meer informatie [Werk bijwerken](note-test.md).


## UGP-10614 - Probleemtabellen met afbeeldingen

Ik denk dat de `{width="20"}` Deze parameter veroorzaakt problemen in tabellen.

## Vergelijking van de succesplannen van Expert en Ultimate

|  | Plan met succes voor experts | Plan voor ultieme successen |
|--- |--- |--- |
|  | Met het Expert Succesplan hebt u toegang tot **24x7 deskundige zorg** voor technische het oplossen van problemen en begeleiding op uw kritieke bedrijfskwesties. Of je vindt snelle oplossingen door te tikken op onze zelfgeleide bronnen, exclusieve best practices en een online gemeenschap van experts en collega&#39;s in de Adobe. <p> *Bij alle Adobe Experience Cloud-licenties inbegrepen.* | Met het Ultimate Success-plan zult u ervaren **strategische begeleiding en proactieve technische gezondheid om hoogwaardige digitale ervaringen te bieden**. Uw milieu van de Adobe zal door een team van deskundigen worden gesteund die met uw zaken vertrouwd zijn en zich op het uitvoeren van een roadmap gericht die op uw doelstellingen en prioriteiten voor bedrijfseffect wordt gericht. |
| **Succesteam** | Samengevoegd team van supporttechnici | Omvat: <ul><li> Aangewezen Technical Account Manager </li><li> Aangewezen Klantsuccesbeheer </li><li> Aangewezen Manager van de Diensten van de Steun</li><li> Gepoold team van technische technici en strategische deskundigen die Succesversnellers leveren </li><li> Samengevoegd team van supporttechnici </li></ul> |
| **Proactieve technische en operationele ondersteuning** | ![niet inbegrepen pictogram](../assets/Cross_red_circle.svg){width="20"} Niet inbegrepen | Omvat: <ul><li>Revisies voor upgrades en migratie, voorbereiding release </li><li>Overzicht van routekaarten voor producten</li><li> Gerichte technische en strategische routekaarten</li><li>Belangrijke voorbereiding en planning van gebeurtenissen</li><li>Planning voor relevante en tijdige activering</li><li>Technische beste praktijken en industriestandaarden</li><li>Aanmoedigen/uitlijnen met productteams</li><li>Uniform plan om belangrijke bedrijfsdoelstellingen te bereiken - Wederzijdse Actieplan (MAP)</li></ul> |
| **Technische ondersteuning** | Omvat: <ul><li>**P1**: 24x7 probleemondersteuning</li><li>**P2, P3, P4**: ondersteuning voor kantooruren</li><li>Standaardoutputbeheer</li><li>Gepoold escalatiebeheer</li></ul> | Omvat: <ul><li>**P1**: 24x7 probleemondersteuning</li><li>**P2/P3**: 24x5-ondersteuning voor uitgaven</li><li>**P4**: ondersteuning voor kantooruren</li><li>Prioritair beheer van uitval</li><li>Aangewezen deskundige escalatiebeheer</li></ul> |
| **Accelerators met succes** | ![niet inbegrepen pictogram](../assets/Cross_red_circle.svg){width="20"} Niet inbegrepen | Succesvolle versnellers die regelmatig door TAM en CSM worden gepland<p>*(zie Accelerator-catalogus met succes voor meer informatie)* |
| **Ondersteuningskanalen** | Online, telefoon, Experience League, forums | Persoonlijk online portaal, telefoon, Experience League, forums met prioriteit |

{style="table-layout:fixed"}

## Support-invoegtoepassingen

| Invoegtoepassingen | Plan met succes voor experts | Plan voor ultieme successen |
|--- |--- |--- |
| **Invoegtoepassing Gebeurtenisbeheer**<br> Biedt end-to-end leiderschap en steun die wordt vereist om de volledige levenscyclus van zeer belangrijke gebeurtenissen te beheren | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Technical Account Director-invoegtoepassing**<br> Uw toonaangevende technische hulpbron die leiderschapstoezicht biedt, de betrokkenheid van managers bezit en het bestuur verzekert om uw bedrijfsresultaten te maximaliseren | ![niet beschikbaar pictogram](../assets/Cross_red_circle.svg){width="20"} Niet beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Geavanceerde invoegtoepassing voor cloudondersteuning**<br> Topservice en waarborg voor klanten van Adobe Experience Manager as a Cloud Service | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar |
| **Invoegtoepassing Mentor Sessions**<br> Verstrekt op vaardigheid-gebaseerd leren in een just-in-time opleidingsmethode | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![beschikbaar pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |
| **Invoegtoepassing ontwikkelaarsverhoging**<br> Verleent toegang tot de deskundigen van de gebiedstechniek die met break-fix werk kunnen helpen | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![inbegrepen pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |
| **Toevoeging van de bundel voor prioritaire wachtrij**<br> Sla de regel over, zodat uw tickets eerst worden bewerkt met extra toegang tot Mentor Sessions en Developer Boost | ![beschikbaar pictogram](../assets/Plus_blue.svg){width="20"} Beschikbaar | ![inbegrepen pictogram](../assets/green_checkmark.svg){width="20"} Opgenomen |

{style="table-layout:fixed"}
