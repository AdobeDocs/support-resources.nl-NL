---
title: Structuur van de in- of uitvoerorganisatie en producttoewijzingen
description: Leer hoe globale beheerders organisatiehiërarchie en producttoewijzingsgegevens in de Global Admin Console exporteren en importeren met JSON, CSV of XLSX. Is van toepassing op ondernemingen.
feature-set: Experience Cloud Services
solution: Admin Console
feature: Admin Console
source-git-commit: fe5b03e5886a43b55929a2bdba45da3c08ad0ab9
workflow-type: tm+mt
source-wordcount: '4375'
ht-degree: 0%

---


# Structuur van de in- of uitvoerorganisatie en producttoewijzingen

**is op van toepassing:** Onderneming

Leer hoe globale beheerders organisatie en productbeheer kunnen stroomlijnen met export- en importfuncties in de Global Admin Console.

Heb toegang tot het **[!UICONTROL Organizations]** lusje in [&#x200B; Global Admin Console &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/adopt-global-administration.html) om de organisatiestructuur uit te voeren of in te voeren. Ga naar het tabblad **[!UICONTROL Product Allocation]** voor toewijzingsgegevens. Gebruik het pictogram **[!UICONTROL More Options]** **⋮** om het exporteren of importeren te selecteren. [&#x200B; Teken binnen aan Global Admin Console &#x200B;](https://global-admin-console.adobe.com).

## De organisatiestructuur exporteren

Als a [&#x200B; globale beheerder &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/manage-administrators.html), kunt u de organisatiehiërarchie uitvoeren. U kunt een JSON-, CSV- of XLSX-representatie van de gehele organisatiehiërarchie of een subset ervan downloaden. U kunt deze gegevens vervolgens gebruiken voor analyse of wijziging.

De gekozen exportindeling is van invloed op de structuur van de geëxporteerde gegevens:

- CSV-indeling — Hiermee kunt u slechts één soort gegevens tegelijk exporteren. Wanneer u productprofielen in CSV-indeling exporteert, worden de profielen en bronnen in één tabel gecombineerd. Er zijn meerdere vermeldingen voor het productprofiel, één voor elke bron.
- XLSX-indeling — Resultaten in elk organisatiedetail die in een apart blad wordt weergegeven. Records worden met een referentie-id verbonden tussen de verschillende objecttypen. In sommige gevallen kunnen er meerdere rijen voor een bepaald object zijn (bijvoorbeeld Bronobjecten wanneer er een set waarden aan een bepaalde bron is gekoppeld).
- JSON-indeling — De meest flexibele indeling. Het kan voordeel halen uit structurele verhoudingen tussen uitgevoerde voorwerpen (bijvoorbeeld, verschijnen de producten in een organisatie direct in het organisatieelement). Dezelfde velden worden in alle drie de indelingen geëxporteerd, maar sommige waarden zijn overbodig in de JSON-indeling.

### Stappen voor exporteren

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/). Op het tabblad **[!UICONTROL Organizations]** gebruikt u de organisatieselectie om de organisatiehiërarchie te selecteren waarin u wilt exporteren. Gegevens voor alle organisaties in de hiërarchie worden geëxporteerd.
2. Selecteer het pictogram **[!UICONTROL More Options]** ⋮ en kies **[!UICONTROL Export]** .

   ![&#x200B; de organisatiestructuur van de Uitvoer &#x200B;](./assets/export-org-structure.png)

3. Selecteer in het dialoogvenster **[!UICONTROL Export]** wat u wilt exporteren en een indeling waarin u de gegevens wilt exporteren.

   ![&#x200B; de uitvoerdialoogdoos van Admin Console &#x200B;](./assets/export-12.png)

4. Selecteer **[!UICONTROL Export]**. Het genereren van het exportbestand kan enkele minuten in beslag nemen. Als u het rapport eenmaal hebt gedownload, navigeert u naar **[!UICONTROL Global Admin Console]** > **[!UICONTROL Insights]** > **[!UICONTROL Export Reports]** .

&#x200B;> [!NOTE]
>
> JSON-bestanden worden geëxporteerd in ZIP-indeling. U kunt ze openen met een ZIP-hulpprogramma of de ZIP-functies van het besturingssysteem.

Nadat u het bestand hebt gedownload, kunt u de gegevens bewerken en vervolgens weer importeren. De geïmporteerde updates worden in de Global Admin Console weergegeven alsof u de gegevens handmatig hebt bewerkt.

## De organisatiestructuur importeren

Als a [&#x200B; globale beheerder &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/manage-administrators.html), kunt u potentieel gewijzigde gegevens invoeren. Bij het uploaden worden de nieuwe gegevens vergeleken met de huidige gegevens en worden eventuele wijzigingen toegepast op de organisatiehiërarchie. Alle importbewerkingen worden uitgevoerd op het bijgewerkte exemplaar van de organisatiehiërarchie. Als u nog wijzigingen aanbrengt, worden de importwijzigingen toegevoegd boven op de wijzigingen die in de hiërarchie in behandeling zijn.

### Te importeren stappen

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com). Op het tabblad **[!UICONTROL Organizations]** gebruikt u de organisatieselectie om de organisatiehiërarchie te selecteren waarin u het importeren wilt uitvoeren.
2. Selecteer het pictogram **[!UICONTROL More Options]** **⋮** en selecteer **[!UICONTROL Import]** . Afhankelijk van de grootte en complexiteit van het importbestand kan de verwerking enkele seconden tot enkele minuten duren.
3. Selecteer **[!UICONTROL Select a file]** en kies een JSON-, CSV- of XLSX-bestand dat u wilt uploaden. Voor CSV kan slechts één organisatiedetails tegelijkertijd worden ingevoerd en het steunt het invoeren van Producten niet. De geïmporteerde wijzigingen lijken alsof u de gegevens handmatig hebt bewerkt.
4. Selecteer **[!UICONTROL Close]**.
5. Selecteer **[!UICONTROL Review Pending Changes]**. Dan, selecteer **[!UICONTROL Submit Changes]** om [&#x200B; uit te voeren &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/execute-jobs.html) hen. Voordat de wijzigingen worden uitgevoerd, worden de acties in behandeling weergegeven op dezelfde manier als wanneer de bewerkingen handmatig worden uitgevoerd in de Global Admin Console.

## Programma&#39;s voor exporteren en importeren

Tijdens het importeren van gegevens met een CSV-bestand kunnen de velden in willekeurige volgorde worden weergegeven, maar moeten ze altijd overeenkomen met de koptekstrij.

Tijdens het importeren van gegevens moet u een bewerking voor elk element opgeven. De bewerking kan een van de volgende handelingen zijn:

- Bijwerken: geeft een bewerking aan.
- Maken: verwijst naar het maken van een nieuw object (bijvoorbeeld organisatie, gebruikersgroep of beheerder).
- Verwijderen: verwijst naar het verwijderen van een object (bijvoorbeeld organisatie, gebruikersgroep of beheerder).

Invoerrecords zonder of leeg bewerkingsveld worden genegeerd.

### Organisaties

<table>
  <tr>
    <th>Veldnaam</th>
    <th>Beschrijving</th>
    <th>Notities</th>
  </tr>

<tr>
    <td>id</td>
    <td>
      Organisatie-id.<br><br>
      Wanneer u een nieuwe organisatie toevoegt, kan dit leeg zijn of bijvoorbeeld worden ingesteld op een plaatsaanduiding-id
      new_org_1. De plaatsaanduiding-id wordt gebruikt in gevallen waarin andere geïmporteerde items moeten verwijzen
      aan deze organisatie. Na het maken wordt een daadwerkelijke organisatie-id toegewezen die alle
      gebruik van de organisatie-id voor plaatsaanduidingen.
    </td>
    <td>Kan op een tijdelijke waarde worden ingesteld wanneer operation=create</td>
  </tr>

<tr>
    <td>name</td>
    <td>
      Organisatie, eenvoudige naam. Minimumlengte 4, max. 100.
      Namen kunnen UTF-8-tekens bevatten, tot 3 bytes.
      4-byte tekens worden niet ondersteund.
    </td>
    <td>
      Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update
    </td>
  </tr>

<tr>
    <td>countryCode</td>
    <td>Code land of regio</td>
    <td>
      Moet worden ingesteld wanneer operation=create, kan worden bijgewerkt wanneer operation=update
    </td>
  </tr>

<tr>
    <td>type</td>
    <td>Type organisatie</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>parentOrgId</td>
    <td>
      Id van bovenliggende organisatie. Leeg voor basisorganisatie.
      Bij het bijwerken zijn er belangrijke beperkingen van toepassing, inclusief dat nieuwe bovenliggende element zich in dezelfde hiërarchie bevindt en
      beschikken over de producten die in de organisatie aanwezig zijn.
    </td>
    <td>
      Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update
    </td>
  </tr>

<tr>
    <td>adminCount</td>
    <td>Aantal beheerders</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>domainCount</td>
    <td>Aantal domeinen</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>userCount</td>
    <td>Aantal gebruikers</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>userGroupCount</td>
    <td>Aantal gebruikersgroepen</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>admins</td>
    <td>Set beheerobjecten die beheerders voor deze organisatie vertegenwoordigt</td>
    <td rowspan="6">
      Mogelijk ontbreekt het als dit niet is geselecteerd voor exporteren. Deze wordt weergegeven op een apart tabblad in XLSX-bestanden.
    </td>
  </tr>

<tr>
    <td>domeinen</td>
    <td>Set domeinobjecten die domeinen in deze organisatie vertegenwoordigen</td>
  </tr>

<tr>
    <td>producten</td>
    <td>Set productobjecten die producten in deze organisatie vertegenwoordigt</td>
  </tr>

<tr>
    <td>productProfiles</td>
    <td>Set productprofielobjecten die productprofielen in deze organisatie vertegenwoordigen</td>
  </tr>

<tr>
    <td>usergroups</td>
    <td>Set gebruikersgroepobjecten die gebruikersgroepen in deze organisatie vertegenwoordigen</td>
  </tr>

<tr>
    <td>orgPolicy</td>
    <td>Structuur die beleid en hun waarden vertegenwoordigt</td>
  </tr>

<tr>
    <td>bewerking</td>
    <td>
      Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd.
    </td>
    <td>Altijd leeg bij exporteren.</td>
  </tr>
</table>


**de vereisten van de Invoer:**

- Voor update of schrapping, moet orgId naar een bestaande organisatie in uw hiërarchie verwijzen.
- Als u een nieuwe organisatie creeert, kunt u het orgId- gebied leeg verlaten of het plaatsen aan unieke identiteitskaart die u (zoals new-1 of new-2) kunt maken. Dit verstrekt identiteitskaart die kan worden gebruikt om naar de te creëren organisatie te verwijzen.
- Landcode moet geldig zijn.
- orgId voor *Update* en *schrapt* verrichting zou reeds in de organisatiehiërarchie moeten aanwezig zijn.
- orgId duidelijk als *Schrapping* zou niet als parentOrgId voor organisaties met *Update* of *moeten worden geselecteerd creeert* verrichting.
- De organisaties van het kind op het zelfde niveau en van de zelfde ouder zouden niet zelfde orgNames moeten hebben.
- Voor het maken van een organisatie of het bijwerken van een organisatienaam, moet de naam van de organisatie niet de naam van een bestaand kind van de zelfde ouder aanpassen.

### Admins

<table>
  <tr>
    <th>Veldnaam</th>
    <th>Beschrijving</th>
    <th>Gebruiken</th>
  </tr>

<tr>
    <td>orgId</td>
    <td>Verwijzing naar de organisatie waarin de beheerder woont.</td>
    <td>Wordt gebruikt als een verwijzing om te zoeken naar omvattende of gekoppelde objecten.</td>
  </tr>

<tr>
    <td>firstName</td>
    <td>
     Voornaam gebruiker beheren.
De voor- en achternaam voor Adobe ID-gebruikers kunnen worden vervangen door een door de gebruiker opgegeven waarde wanneer de gebruiker de uitnodiging accepteert.
    </td>
    <td rowspan="4">
      Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update
    </td>
  </tr>

<tr>
    <td>lastName</td>
    <td>Achternaam Admin-gebruiker</td>
  </tr>

<tr>
    <td>email</td>
    <td>E-mailadres van gebruiker beheren. Dit is een primaire sleutel voor de gebruiker en moet uniek zijn.</td>
  </tr>

<tr>
    <td>countryCode</td>
    <td>
Land- of regiocode waar de gebruiker werkt. Alleen van toepassing op de typen federatieve id en Enterprise-id.
    </td>
  </tr>

<tr>
    <td>userType</td>
    <td>Een van "Adobe ID", "Enterprise ID" of "Federated ID".</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>adminType</td>
    <td>Één van "GLOBAL ADMIN", "GLOBAL VIEWER", "SYSTEM ADMIN", "USER GROUP ADMIN", "PRODUCT ADMIN", "PRODUCT PROFILE ADMIN", "IMPLOYMENT ADMIN", en "STORAGE_ADMIN".</td>
    <td rowspan="4">Kan worden ingesteld wanneer operation=Create</td>
  </tr>

<tr>
    <td>groupId</td>
    <td>Groep-id van groep waarvan deze gebruiker een beheerder is. Alleen relevant voor gebruikers- en productprofielbeheerders.</td>

</tr>

<tr>
    <td>licenseId</td>
    <td>Product license id of the product this user is admin of. Alleen relevant voor productbeheerders.</td>

</tr>

<tr>
    <td>domein</td>
    <td>Domeinnaam van gebruiker indien geen e-maildomein wordt gebruikt</td>

</tr>

<tr>
    <td>userName</td>
    <td>Gebruikersnaam van gebruiker indien geen e-mailadres wordt gebruikt</td>
    <td></td>
  </tr>

<tr>
    <td>bewerking</td>
    <td>Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd.</td>
    <td></td>
  </tr>
</table>


**de vereisten van de Invoer:**

- orgId, email, adminType en userType moeten geldige waarden bevatten.
- countryCode moet geldig zijn.
- Als de gebruiker al bestaat en wordt bijgewerkt, moet userType aan de gebruiker aanpassen.
- Controleren op dubbele e-mailadressen in de organisatie.

### Productprofielen

De uitvoer en de invoer van productprofielen bestaan uit twee delen: de details van het productprofiel, en een reeks middelen verbonden aan het productprofiel. Deze middelen identificeren de diensten die kunnen worden gevormd, gewoonlijk enkel om hen toe te laten of onbruikbaar te maken.

- De bronobjecten worden in JSON-indeling in het productprofiel genest.
- Als u CSV of XLSX gebruikt met productprofielen, worden de profielen en bronnen in één tabel gecombineerd. Er zijn meerdere vermeldingen voor het productprofiel, één voor elke bron.
- Het &quot;geselecteerde&quot;gebied in het middel controleert of de dienst wordt toegelaten.
- Wanneer u productprofielen importeert, moet de bewerking Maken of Bijwerken worden uitgevoerd op het productprofiel zelf en op alle bronobjecten die moeten worden bijgewerkt of gemaakt.


<table>
  <tr>
    <th>Veldnaam</th>
    <th>Beschrijving</th>
    <th>Gebruiken</th>
  </tr>

<tr>
    <td>productProfileId</td>
    <td>
     <br><br>
      Identificatiecode van het productprofiel
U kunt plaatsaanduidingswaarde gebruiken bij maken, zodat andere objecten naar het nieuwe profiel kunnen verwijzen.
    </td>
    <td>Kan op tijdelijke waarde worden ingesteld wanneer operation=create</td>
  </tr>

<tr>
    <td>productProfileName</td>
    <td>
     Naam van productprofiel. Het kan geen duplicaat zijn van andere productprofielen of gebruikersgroepen in dezelfde organisatie.
    </td>
    <td rowspan="2">
   Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update
    </td>
  </tr>

<tr>
    <td>productProfileDescription</td>
    <td>Tekstbeschrijving van het productprofiel</td>
  </tr>

<tr>
    <td>licenseId</td>
    <td>Referentie van licentie-id voor het product</td>
    <td rowspan="2"> Wordt gebruikt als een verwijzing om te zoeken naar een object dat het object bevat of eraan is gekoppeld
    </td>
  </tr>

<tr>
    <td>orgId</td>
    <td>
Organisatie die de gebruikersgroep bevat
    </td>
  </tr>

<tr>
    <td>meldingen</td>
    <td>Waar of onwaar om aan te geven of e-mailbericht naar gebruikers moet worden verzonden wanneer ze uit dit productprofiel worden toegevoegd of verwijderd</td>
    <td>Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update</td>
  </tr>

<tr>
    <td>bronnen</td>
    <td> Array met bronnen die aan dit productprofiel zijn gekoppeld.
Het veld Resources is alleen aanwezig voor de JSON-indeling. Voor CSV en XLSX formaat, worden de middelen vertegenwoordigd met de volgende extra gebieden: resourceName, resourceId, resourceDescription, icon, selected, quota, resourceType. Zie [Producten en bronnen](#products-and-resources) voor meer informatie over deze velden.
Als het productprofiel meer dan één bron heeft, zijn er meerdere rijen aanwezig, één voor elke bron. De andere velden hebben dezelfde waarden voor elke bron. </td>
    <td></td>
  </tr>

<tr>
    <td>bewerking</td>
    <td>Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd.</td>  
    <td></td>
  </tr>
</table>



**de vereisten van de Invoer:**

- productProfileId, licenseId en orgId moeten geldige waarden hebben.
- Wanneer u een productprofiel maakt, moet de productProfileName een geldige naam zijn en mag deze geen andere productprofielnaam of gebruikersnaam in dezelfde organisatie dupliceren.
- Het quotaveld moet een geldige waarde hebben voor het eenheidstype. Dit is numeriek of &quot;onbeperkt&quot;wanneer resourceType=QUOTA of anders leeg.
- Het berichtveld moet waar of onwaar zijn.
- Voor CSV- en XLSX-import moet u productProfileId valideren. Alle vermeldingen moeten dezelfde orgId, licenseId en productProfileName hebben.
- Valideer dubbel productProfileName in het inputdossier en de organisatie.
- Profielen die moeten worden bijgewerkt en verwijderd, moeten aanwezig zijn in de organisatie.
- Middelen die moeten worden bijgewerkt en verwijderd (gedeactiveerd), moeten in het profiel aanwezig zijn.
- Controleer het volgende voor profielen die moeten worden gemaakt:
   - orgId zou een nieuwe organisatie of een bestaande organisatie moeten zijn.
   - De licentie-id moet een nieuw product of een bestaand product zijn.
   - Valideer de bronnen voor het profiel.

### Bronnen in productprofielen


<table>
  <tr>
    <th>Veldnaam</th>
    <th>Beschrijving</th>
    <th>Gebruiken</th>
  </tr>

<tr>
    <td>resourceName</td>
    <td>
     Naam van de bron
    </td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>resourceId</td>
    <td>
   Identificatiecode van de bron
    </td>
    <td>
   Alleen-lezen
    </td>
  </tr>

<tr>
    <td>resourceDescription</td>
    <td>Tekstbeschrijving van de bron</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>pictogram</td>
    <td>URL naar afbeelding voor bron</td>
    <td> Alleen-lezen</td>
  </tr>

<tr>
    <td>geselecteerd</td>
    <td>Voor een configuratieingang, of de eigenschap wordt toegelaten. Dit veld is alleen beschikbaar in JSON.</td>
    <td rowspan ="2">Kan worden ingesteld of bijgewerkt wanneer operation=create of operation=update.</td>
  </tr>

<tr>
    <td>quota</td>
    <td>Hoeveelheid primaire bron die via dit productprofiel aan gebruikers kan worden verstrekt. Dit veld is alleen beschikbaar in JSON.</td>
    <td></td>
  </tr>

<tr>
    <td>resourceType</td>
    <td> Indien aanwezig, is de waarde SERVICE. Deze resource geeft een service aan die op basis van de waarde van het geselecteerde veld kan worden in- of uitgeschakeld. Dit veld is alleen beschikbaar in JSON.</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>bewerking</td>
    <td>Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd.</td>  
    <td></td>
  </tr>
</table>

**de vereisten van de Invoer:**

- Het gebied van de verrichting op middelen wordt genegeerd wanneer het productprofiel waartot zij behoren verrichtingen heeft die als *worden geplaatst schrapt* of *creeert*.
- Geen middel zou voor schrapping moeten worden gemerkt; het is een ongeldige verrichting.
- Voor productprofielen die moeten worden gemaakt, moet het aantal bronnen overeenkomen met het aantal bronnen van het bronproductprofiel.
- Voor middelen met *Update* verrichting, moet het middel in het productprofiel aanwezig zijn.

### Gebruikersgroepen

<table>
  <tr>
    <th>Veldnaam</th>
    <th>Beschrijving</th>
    <th>Gebruiken</th>
  </tr>

<tr>
    <td>userGroupId</td>
    <td>
Id van gebruikersgroep
U kunt plaatsaanduidingswaarde gebruiken bij maken, zodat andere objecten naar de nieuwe gebruikersgroep kunnen verwijzen.
    </td>
    <td>Kan op tijdelijke waarde worden ingesteld wanneer operation=create</td>
  </tr>

<tr>
    <td>userGroupName</td>
    <td> Naam van gebruikersgroep</td>
    <td rowspan="2"> Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update</td>
  </tr>

<tr>
    <td>userGroupDescription</td>
    <td>Tekstbeschrijving van gebruikersgroep</td>
    <td></td>
  </tr>

<tr>
    <td>userCount</td>
    <td>Aantal gebruikers in gebruikersgroep</td>
    <td>Alleen-lezen</td>
  </tr>

<tr>
    <td>profielen</td>
    <td>Array met productprofielid's waaraan de gebruikersgroep is gekoppeld.
XLSX heeft één rij per waarde met dezelfde waarden voor andere velden.</td>
    <td>Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update</td>
  </tr>

<tr>
    <td>orgId</td>
    <td>Organisatie die de gebruikersgroep bevat.</td>
    <td>Wordt gebruikt als een verwijzing om te zoeken naar een object dat het object bevat of eraan is gekoppeld.</td>
  </tr>

<tr>
    <td>bewerking</td>
    <td>Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd.</td>
    <td></td>
  </tr>
</table>



**de vereisten van de Invoer:**

- orgId moet verwijzen naar een bestaande organisatie of een organisatie die in de zelfde invoer wordt gecreeerd.
- userGroupId moet verwijzen naar een bestaande groep voor update of schrapping, en kan identiteitskaart zijn u voor nieuwe gebruikersgroepen bepaalt.
- Voor update of aanmaak mag userGroupName niet leeg zijn en mag deze een andere gebruikersgroep of productprofielnaam in dezelfde organisatie niet dupliceren.
- Zorg ervoor dat userGroupName niet wordt gedupliceerd in het invoerbestand en de organisatie.
- gebruikersgroepen die moeten worden bijgewerkt en verwijderd, moeten aanwezig zijn in de organisatie.
- Profiel dat moet worden verwijderd uit gebruikersgroep, moet aanwezig zijn in de gebruikersgroep. U kunt updatebewerkingen niet uitvoeren op het profiel van een gebruikersgroep.
- Zorg ervoor dat voor gebruikersgroepen die u wilt maken:
   - orgId zou een nieuwe organisatie of een bestaande organisatie moeten zijn.
   - De licentie-id moet, indien van toepassing, een nieuw product of een bestaand product zijn.
   - De productProfileId moet een nieuw productprofiel of een bestaand productprofiel zijn.

### Domeinen

De domeininformatie verstrekt read-only informatie over domeinen beschikbaar in elke organisatie. Deze gegevens kunnen niet worden bewerkt.


| Veldnaam | Beschrijving | Gebruiken |
| ------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| orgId | Verwijzing naar de organisatie waarin dit domein is vermeld | Wordt gebruikt als een verwijzing om te zoeken naar omvattende of gekoppelde objecten. |
| domainName | Naam van het domein (bijvoorbeeld adobe.com). | Alleen-lezen |
| directoryName | Naam van de map waarin het domein wordt vermeld | Alleen-lezen |
| directoryType | Een van Federated ID of Enterprise ID. | Alleen-lezen |
| domainStatus | Een van de opties &quot;ACTIEF&quot;, &quot;RESERVED&quot;, &quot;UNCLAIMED&quot;, &quot;CLAIMED&quot;, &quot;VALIDATED&quot;, &quot;WITHDRAWN&quot;, &quot;EXPIRED&quot;. | Alleen-lezen |


### Producten en hulpbronnen {#products-and-resources}

In XLSX-bestanden zijn er twee bladen: één voor producten en één voor de bronnen. In JSON worden bronobjecten genest in het productobject.

**Producten**


| Veldnaam | Beschrijving | Gebruiken |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| licenseId | Id die het product identificeert. Elk product heeft een unieke licentie-id in de organisatie waarin het wordt vermeld. Wanneer u een nieuw product toevoegt, kan dit leeg zijn of een plaatsaanduiding-id gebruiken (bijvoorbeeld new_product_1). Na het maken wordt een werkelijke licentie-id toegewezen die alle toepassingen van de tijdelijke aanduiding voor de licentie-id vervangt. | Kan op tijdelijke waarde worden ingesteld wanneer operation=create |
| productName | Naam van het product | Alleen-lezen |
| productDescription | Tekstbeschrijving van het product | Alleen-lezen |
| allowOverassign | Booleaanse waarde die aangeeft of overtoewijzing van dit productexemplaar is toegestaan. Overallocatie heeft betrekking op de mogelijkheid om meer aan een kinderorganisatie toe te kennen dan u hebt toegekend. | Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update |
| pictogram | URL van productpictogram | Alleen-lezen |
| sourceLicenseId | Licentie-id van productinstantie in de organisatie waaruit dit product is toegewezen. Waarde is null als deze instantie geen toegewezen product is, maar een aangeschaft product. | Kan worden ingesteld wanneer operation=Create |
| productId | Identificatiecode van het product. | Alleen-lezen |
| orgId | Identificatiecode van de organisatie die deze productinstantie bevat | Wordt gebruikt als een verwijzing om te zoeken naar een object dat het object bevat of eraan is gekoppeld |
| herverdelbaar | Booleaanse waarde die aangeeft of dit product bronnen heeft die kunnen worden toegekend aan onderliggende organisaties. | Alleen-lezen |
| bronnen | Object dat een set bronobjecten bevat die de bronnen en instellingen in dit product vertegenwoordigt |                                                                               |
| bewerking | Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd. |                                                                               |


**de vereisten van de Invoer:**

- Voor het maken moet de licentie-id een unieke id zijn die u maakt.
- Voor update moet de licentie-id de id zijn van een bestaand product in de opgegeven organisatie.
- orgId moet verwijzen naar een bestaande organisatie of een organisatie die in de zelfde de invoerverrichting wordt gecreeerd.
- Voor het maken moet sourceLicenseId verwijzen naar een bestaand product of de id die u hebt gedefinieerd voor een product dat wordt gemaakt in dezelfde importbewerking.
- licenseId en sourceLicenseId zouden niet het zelfde voor producten met *moeten zijn creeer* verrichting.
- Gevalideerde organisaties van producten; de organisatie zou nieuw moeten zijn of zou reeds in de organisatiehiërarchie moeten aanwezig zijn.
- Voor *Update* en *schrapt* verrichting, zou het product reeds in de organisatiehiërarchie moeten aanwezig zijn.
- licenseId duidelijk als *Schrapping* zou niet als sourceLicenseId van producten met *moeten worden gebruikt creeer* en *Update* verrichting.
- Voor producten met *creëren* verrichting, bevestig dat sourceLicenseId in de ouderorganisatie aanwezig zou moeten zijn.

**Middelen voor producten**

Bronobjecten kunnen in producten en in productprofielen worden weergegeven.


| Veldnaam | Beschrijving | Gebruiken |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| resourceName | Naam van de bron | Alleen-lezen |
| resourceId | Identificatiecode van de bron | Alleen-lezen |
| resourceDescription | Tekstbeschrijving van de bron | Alleen-lezen |
| pictogram | URL naar afbeelding voor bron | Alleen-lezen |
| productName | De naam van het product waarvan deze resource deel uitmaakt. | Alleen-lezen |
| licenseId | Licentie-id (productinstantie) van het product waarvan deze resource deel uitmaakt. | Wordt gebruikt als een verwijzing om te zoeken naar een object dat het object bevat of eraan is gekoppeld |
| allowedQuantity | Toegewezen hoeveelheid van deze bron: hoeveelheid middelen die deze organisatie ter plaatse kan gebruiken of toewijzen aan onderliggende organisaties. | Kan worden ingesteld of bijgewerkt wanneer respectievelijk operation=create of operation=update |
| eenheid | Naam van de eenheid van de subsidiehoeveelheid. | Alleen-lezen |
| currentQuantity | Huidige bruikbare hoeveelheid in deze organisatie. Dit is de toegekendeHoeveelheid minder middelen die aan kindorganisaties worden toegewezen. Dit is de waarde die wordt weergegeven in de Admin Console voor dit product/deze bron. | Alleen-lezen |
| provisionedQuantity | Aantal werkelijk provisioned: kan kleiner zijn dan subsidie of stroom, kan minder zijn dan currentQuantity als één of andere beperking op zijn plaats is. | Alleen-lezen |
| bewerking | Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd. |                                                                               |


**de vereisten van de Invoer:**

Het gebied van de verrichting op middelen wordt genegeerd wanneer het product waartot zij behoren verrichtingen heeft die als *worden geplaatst schrapt* of *creeert*.
- Geen middel zou voor schrapping moeten worden gemerkt; het is een ongeldige verrichting.
- Voor te creëren producten, zou het aantal middelen het aantal middelen van het bronproduct moeten aanpassen.
- Voor middelen met *Update* verrichting, moet het middel in het product aanwezig zijn.

## Gegevens over de toewijzing van producten bij invoer en uitvoer

Als a [&#x200B; Globale Beheerder &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/manage-administrators.html), kunt u de gegevens van de producttoewijzing als JSON of Csv- dossier uitvoeren. U kunt deze gegevens vervolgens bewerken en uploaden om de wijzigingen te importeren. Wanneer de potentieel gewijzigde gegevens worden geüpload, worden de nieuwe gegevens vergeleken met de huidige gegevens en worden eventuele wijzigingen toegepast op de producttoewijzingsgegevens. Vervolgens kunt u de wijzigingen die in behandeling zijn bekijken en verzenden voordat deze van kracht worden.

## Het model voor producttoewijzing exporteren

Ga als volgt te werk om het producttoewijzingsmodel te exporteren:

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/) en navigeer aan het **[!UICONTROL Product Allocation]** lusje.
2. Selecteer het pictogram **[!UICONTROL More Options]** ⋮ en selecteer vervolgens **[!UICONTROL Export CSV]** of **[!UICONTROL Export JSON]** . Het bestand is gedownload. [&#x200B; leer meer &#x200B;](#export-and-import-formats-for-product-allocation) over de de uitvoerformaten.

## Het model voor producttoewijzing importeren

U kunt gegevens exporteren, wijzigen en vervolgens het gewijzigde bestand importeren. Ga als volgt te werk om het producttoewijzingsmodel te importeren:

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/) en navigeer aan het **[!UICONTROL Product Allocation]** lusje.
2. Selecteer het pictogram **[!UICONTROL More Options]** ⋮ en selecteer **[!UICONTROL Import]** .
3. Selecteer een JSON- of CSV-bestand dat u wilt uploaden.
4. Selecteer **[!UICONTROL Review Pending Changes]**. Na het herzien van de veranderingen, uitgezocht **[!UICONTROL Submit Changes]** om [&#x200B; uit te voeren &#x200B;](https://helpx.adobe.com/nl/enterprise/global-admin-console/execute-jobs.html) hen.

## Indelingen voor uitvoer en invoer voor producttoewijzing

De uitvoer- en importindelingen zijn hetzelfde. Tijdens het importeren in CSV-indeling kunnen de velden in elke willekeurige volgorde worden weergegeven, maar moeten ze overeenkomen met de koptekstrij. Tijdens het importeren in JSON-indeling kunnen de velden in elke gewenste volgorde worden weergegeven.

U moet de bewerking opgeven tijdens het importeren van de gegevens voor producttoewijzing. De bewerking kan een van de volgende zijn:

- Update: geeft een bewerking aan (wijziging in de waarden allowedQuantity, allowOverAllocation).
- Maken: geeft aan dat een productbron aan de opgegeven organisatie moet worden toegevoegd.
- Verwijderen: hiermee wordt het verwijderen van een product aangegeven.

Als er geen bewerking is opgegeven, worden er geen wijzigingen aangebracht wanneer gegevens voor die rij worden geïmporteerd in CSV of in JSON.

In het geëxporteerde bestand is er één rij of record voor elke bron van het product. Sommige producten hebben meer dan één bron.

Als een product meer dan één bron heeft, kunnen de verrichtingen van de Update op onafhankelijke middelen van toepassing zijn, schrapt een verrichting van de Schrapping het product met inbegrip van alle middelen van een organisatie, en creeert verrichting vereist een verslag voor elk van de middelen in het de invoerdossier zodat de juiste hoeveelheid van elk van hen kan worden gespecificeerd. Het veld allowOverAllocation is voor het hele product en het maakt niet uit in welke bron een update voor dit veld zich bevindt.

### Beschrijving van kopteksten


| Veldnaam | Beschrijving | Gebruiken |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| productName | Naam van het product. | Alleen-lezen |
| licenseId | Id van een product (uniek voor een product in een organisatie). Wanneer u een nieuw product toevoegt, kan dit leeg zijn of op een plaatsaanduiding-id worden ingesteld (bijvoorbeeld new_product_1). De plaatsaanduiding-id wordt gebruikt wanneer andere geïmporteerde items naar dit product moeten verwijzen. Na het maken wordt een werkelijke licentie-id toegewezen die alle toepassingen van de tijdelijke aanduiding voor de licentie-id vervangt. | Kan worden ingesteld wanneer operation=Create |
| sourceLicenseId | Id van bovenliggend product. De waarde is leeg of null als deze een aankoop in plaats van een toewijzing vertegenwoordigt. | Kan worden ingesteld wanneer operation=Create |
| productId | Id die deze productklasse identificeert. Deze id wordt gedeeld door producten van hetzelfde type en verschilt van de licenseId die een instantie van dit product identificeert. | Alleen-lezen |
| resourceName | Naam van deze productbron. Bijvoorbeeld gebruikerslicenties. | Alleen-lezen |
| resourceId | Id die deze productbron identificeert. | Kan worden ingesteld wanneer operation=Create |
| orgPathName | De padnaam van de organisatie waarin deze bron zich bevindt. Segmenten gescheiden door &quot;/&quot;. | Alleen-lezen |
| orgName | Eenvoudige naam van de organisatie die deze productbron bevat. Dit is het definitieve segment van orgPathName. | Alleen-lezen |
| orgId | Organisatie-id van de organisatie die deze productbron bevat. | Kan worden ingesteld wanneer operation=Create |
| allowedQuantity | Aantal eenheden van de hoeveelheid middelen die door de moedermaatschappij aan deze organisatie is toegekend of het aangekochte bedrag als dit product een aankoop vertegenwoordigt. Dit veld kan worden bijgewerkt, behalve voor aangeschafte producten of hoofdtoewijzingen die de algemene beheerder niet mag wijzigen. | Kan worden bijgewerkt wanneer operation=Update of operation=Create |
| eenheid | Naam van de hulpbroneenheid. Bijvoorbeeld Users. | Alleen-lezen |
| totalAllocations | Som van de subsidies aan kindorganisaties van deze organisatie voor dit productmiddel. Deze waarde omvat de rechtstreekse subsidies aan directe kinderen plus overtoewijzingen door die organisaties. Bijvoorbeeld, als deze organisatie een kind 10 verleende en het kind dan zijn kind 25 toewees, zou totalAllocations 25 zijn: de 10 die aan het kind plus een ouder van 15 in dat kind wordt verleend. | Alleen-lezen |
| GrantOverage | Bedrag waarmee totalAllocations de allowedQuantity overschrijdt. Als totalAllocations de allowedQuantity niet overschrijdt, is deze waarde ongeldig of nul. | Alleen-lezen |
| localLicedQuantity | Bedrag van deze middelen die aan deze organisatie zijn toegekend en die voor haar gebruik zijn overgebleven nadat de aan kinderen toegewezen hoeveelheid is afgetrokken. Dit is het bedrag dat beschikbaar is in de Admin Console. Deze waarde kan nul zijn maar is nooit negatief zelfs als deze organisatie middelen aan zijn kinderen heeft oververdeeld. | Alleen-lezen |
| localUsage | Aantal eenheden van de bron die in deze organisatie wordt gebruikt. Bijvoorbeeld, zou het delegeren van een Vergunning van de Gebruiker aan een gebruiker als 1 eenheid van gebruik tellen. | Alleen-lezen |
| totalUsage | Aantal eenheden van het middel dat door deze organisatie en alle kinderen wordt gebruikt. Dit toont gebruik van dit middel in het gedeelte van de organisatiehiërarchie die door deze organisatie wordt geworteld. | Alleen-lezen |
| useOverage | Bedrag van het totale gebruik van de subsidie van de organisatie (organisatie en kinderen hebben meer van de beschikbare middelen gebruikt). Dit toont een waarde niet nul wanneer totalUsage localLicedQuantity overschrijdt. | Alleen-lezen |
| allowOverAllocation | Geeft aan of de gebruiker meer middelen mag toekennen aan kinderen, ook al is er geen subsidie meer (toegestaan ondanks subsidieoverschrijding). Deze waarde is van toepassing op alle bronnen van dit product. Als wordt gepoogd allowOverassign voor meer dan één middel van het zelfde product aan verschillende waarden bij te werken, is het resultaat willekeurig. | Kan worden bijgewerkt wanneer operation=Update |
| isPurchasedProduct | true als het product een aankoopproduct is (niet door de moedermaatschappij toegewezen). Dit is gelijk aan sourceLicenseId met een lege waarde. | Alleen-lezen |
| herverdelbaar | Waar als het product aan kinderen kan worden toegewezen, vals betekent dat het product slechts beschikbaar is in de organisatie waarin het wordt getoond en de middelen niet aan een andere organisatie kunnen worden toegewezen. | Alleen-lezen |
| bewerking | Een van de lege waarden Maken, Bijwerken of Verwijderen. Actie die moet worden uitgevoerd wanneer gegevens worden geïmporteerd. |                                                          |


**de vereisten van de Invoer**

**de bevestiging van Gegevens**

- Het bewerkingsveld moet een geldige bewerking hebben.
- De gegevens over het importeren van producten moeten eigenschappen en waarden hebben voor de vereiste velden.
- De eigenschappen van de productimportgegevens moeten van het juiste type zijn.
- Het veld productbeleid (overAllocation) mag niet voor verschillende bronnen worden opgegeven.
- Het veld allowedQuantity:
   - Kan niet in *onbeperkt* worden veranderd als het niet reeds *onbeperkt* is.
   - Moet een niet-negatief geheel of de koordwaarde *onbeperkt zijn.*

**Toestemming/toegankelijke bevestiging**

- De organisatie die is gekoppeld aan de importgegevens moet bestaan. Als u bijwerkt, moet u ervoor zorgen dat het product en de bron die aan de importgegevens zijn gekoppeld, ook daadwerkelijk bestaan.

**voeg productbevestiging** toe

- SourceLicenseId moet bestaan.
- De organisatie die bij het nieuwe product hoort, moet bestaan.
- Het product dat wordt gemaakt, mag niet bestaan (product met dezelfde licentie-id).
- De middelen verbonden aan een product dat moet hebben een overeenkomstige productId die dat product aanpast.

