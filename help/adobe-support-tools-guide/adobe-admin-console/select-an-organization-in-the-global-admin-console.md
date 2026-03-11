---
title: Een organisatie selecteren in de Global Admin Console
description: Leer hoe u een organisatie kiest voor bewerking in de Global Admin Console.
Feature-set: Experience Cloud Services
Solution: Admin Console
Feature: Admin Console
source-git-commit: 0bc0dbd8c7040e0be7e7bd45945edb0fb24cb7cc
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Een organisatie selecteren in de Global Admin Console

Leer hoe u een organisatie kiest voor bewerking in de Global Admin Console.

>[!NOTE]
>
>Nadat u toegang tot [ Global Admin Console ](https://helpx.adobe.com/enterprise/global-admin-console/adopt-global-administration.html#request-access) hebt, kunt u beginnen door een organisatie te selecteren om de naam van de organisatie, gebruikersgroepen, productprofielen, beheerders, en organisatiebeleid te bekijken en te beheren. Om binnen aan Global Admin Console te ondertekenen, [ klik hier ](https://global-admin-console.adobe.com/).

De Global Admin Console fungeert als centrale beheerhub van de organisatie voor Adobe-middelen. Globale beheerders kunnen:

- Onderliggende organisaties onder hun organisatie aanmaken
- Systeembeheerders toewijzen om deze te beheren
- Verdeel middelen aan kindorganisaties voor beheer en toewijzing aan gebruikers in die organisaties

>[!NOTE]
>
> De gebruikers en de beheerders in een organisatie hebben geen zicht aan gebruikers, opslag, of andere middelen buiten hun organisatie.

## Selecteer uw organisatie

De organisaties die in de **[!UICONTROL organization selector]** drop-down lijst worden vermeld zijn die u uitdrukkelijk een globale admin van-namelijk bent, werd u toegevoegd aan de lijst van beheerders voor die organisatie met een globale admin of globale kijkersrol die. U bent impliciet een algemene beheerder (of algemene viewer) van alle organisaties onder dat punt in de hiërarchie, maar die organisaties worden niet vermeld in [!UICONTROL org picker] .

![ de plukker van de Org ](/help/adobe-support-tools-guide/assets/org-picker.png)

Als u deze wilt weergeven, voegt u uzelf als algemeen beheerder toe aan de organisaties die u wilt weergeven. Wanneer u een org selecteert in [!UICONTROL organization selector], zijn uw administratieve toestemmingen gebaseerd op het zijn van een globale beheerder van de geselecteerde organisatie. U zou ook als globale beheerder van een ouderorganisatie hoger in de boom kunnen worden vermeld, die u meer toestemmingen zou kunnen geven. U moet die organisatie op hoger niveau selecteren om de extra toestemmingen te krijgen.

Nadat u in de Global Admin Console een organisatie hebt geselecteerd in de [!UICONTROL hierarchy tree] , kunt u beginnen met het bewerken van gegevens voor een bepaalde organisatie.

**geeft uit kan beïnvloeden:**

- Naam organisatie
- Gebruikersgroepen
- Productprofielen
- Beheerders
- Organisatiebeleid

**uitgeeft kan niet beïnvloeden:**

- Gebruikers (behalve voor het verwijderen van groepen of productprofielen)
- Gebruikers toevoegen (behalve beheerders)

Wanneer een organisatie is geselecteerd in de hiërarchiestructuur, wordt de volgende informatie weergegeven:

- Naam organisatie
- Regio
- Aantal gebruikers
- Lijst van producten
- Productprofielen
- Gebruikersgroepen
- Beheerders
- Gevraagde domeinen
- Beleidswaarden van de organisatie

Om producten, gebruikersgroepen, beheerders, domeinen, beleid, of beleidsmalplaatjes te bekijken of uit te geven, selecteer het aangewezen lusje. In de meeste gevallen kunt u het veld [!UICONTROL search] gebruiken om een specifiek item op het tabblad te zoeken.

![ geef een organisatie ](/help/adobe-support-tools-guide/assets/edit-an-organization.png) uit

Alle beheerders die aan een org zijn toegevoegd of van een org zijn verwijderd, ontvangen een e-mailbericht. Bepaalde beleidswijzigingen in een org resulteren in een melding in het [!DNL Admin Console] van die organisatie.

## Meer informatie over de beperkingen en noodzakelijke voorwaarden

- De maximale diepte voor nestingorganisaties is vijf. a/b/c/d/e is dus toegestaan, maar a/b/c/d/e/f is een fout. Acme Corp/International Region/Acme Europe/Acme UK/Acme London is bijvoorbeeld toegestaan, maar Acme Corp/International Region/Acme Europe/Acme UK/Acme London/Acme Mayfair is een fout.

- De maximale padnaamlengte (inclusief alle organisaties) is 255 tekens (inclusief &quot;/&quot;). De maximale lengte voor één org-naam ligt tussen 4 en 100 tekens.

- De organisatie pathname is uniek, maar de eenvoudige naam is slechts uniek onder zijn siblings. Er kunnen organisaties zijn met dezelfde eenvoudige naam elders in de hiërarchie van de org.

- U kunt de lijst met domeinen die zijn gekoppeld aan de geselecteerde organisatie alleen weergeven met de algemene beheerconsole. Als u een systeembeheerder van de geselecteerde organisatie bent, selecteer **[!UICONTROL Open in Admin Console]** om domeinen [ te beheren ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html). Om de informatie te begrijpen die in het lusje van Domeinen wordt getoond, zie [ uitvoer en invoerschema&#39;s ](https://helpx.adobe.com/enterprise/global-admin-console/export-and-import-data.html#export-and-import-schemas).

- IE 11 wordt niet gesteund voor globale beleidstoegang. Gebruik een andere browser of een nieuwere versie van de IE-browser.
