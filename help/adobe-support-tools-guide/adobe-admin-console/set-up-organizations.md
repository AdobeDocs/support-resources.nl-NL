---
title: Organisatiehiërarchie beheren
description: Leer hoe globale beheerders de hiërarchie van de organisatie in de Global Admin Console kunnen beheren.
Feature-set: Experience Cloud Services
Solution: Admin Console
Feature: Admin Console
source-git-commit: 3b3b2711887f0db086e4eb8281344cc7356accf7
workflow-type: tm+mt
source-wordcount: '1578'
ht-degree: 0%

---

# Organisatiehiërarchie beheren

Is van toepassing op ondernemingen.

Leer hoe globale beheerders de hiërarchie van de organisatie in de Global Admin Console kunnen beheren.

Nadat u [&#x200B; toegang tot  [!DNL Global Admin Console] krijgt &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/adopt-global-administration.html#request-access), kunt u nieuwe organisaties tot stand brengen, bestaande organisaties aan de hiërarchie toevoegen, organisaties schrappen, en een ouderorganisatie veranderen.
[&#x200B; Teken binnen aan de Global Admin Console &#x200B;](https://global-admin-console.adobe.com/)

Een organisatie is een structuur die wordt gebruikt om Adobe-producten en -gebruikers te beheren. [[!DNL Adobe Admin Console] &#x200B;](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) laat beheerders de plaatsing en de configuratie van producten en gebruikers in hun organisatie beheren. Met [[!DNL Global Admin Console] &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/overview.html) kunnen globale beheerders meerdere organen maken, beheren en verwijderen.

## Een onderliggende organisatie maken

Als a [&#x200B; globale beheerder &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/manage-administrators.html), kunt u kindorganisaties van om het even welke organisatie in de hiërarchie tot stand brengen en de naam, het land, de gebruikersgroepen, de producten, de productprofielen, de beheerders, en het beleid plaatsen.

Wanneer een nieuwe kindorganisatie wordt gecreeerd, worden het volgende automatisch geërft van de directe ouder:

- Het beleid van de organisatie [&#x200B; &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html) montages (met inbegrip van sloten als heden).
- De lijst van systeembeheerders (die door het **[!UICONTROL Inherit System Admins on creation]** [&#x200B; wordt gecontroleerd beleid &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html)).
Het volgende kan systeembeheerders verhinderen worden geërft:
   - Gebrek van [&#x200B; domeinvertrouwen &#x200B;](https://helpx.adobe.com/enterprise/using/directory-trust.html).
   - Beperkingen voor gebruikerstypen (beleid voor Adobe ID/Enterprise ID/Federated ID-gebruikers toevoegen). Leer over de [&#x200B; beleidsdetails &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html).
- Toegang tot [[!DNL Federated ID]] of [[!DNL Enterprise ID]] gebruikers van domeinen waartoe de bovenliggende org toegang heeft. Hierdoor zijn de domeingebruikers in het bovenliggende domein beschikbaar op de onderliggende org. Overerving van gebruikerstoegang wordt gecontroleerd door **erven gebruikers van folders die door de ouderorganisatie** worden beheerd [&#x200B; beleid &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html).
- Het delen van beleid, wachtwoordbeleid, en veiligheidscontacten (die door **worden gecontroleerd erven activa delend montages wanneer de kindorganisatie** [&#x200B; beleid &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html) wordt gecreeerd).

1. Teken binnen aan de [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/). Selecteer op het tabblad **[!UICONTROL Organizations]** de organisatie waaraan u een onderliggende organisatie wilt toevoegen.
2. Selecteer het pictogram **[!UICONTROL Add+]**.
   ![&#x200B; voeg Organisatie &#x200B;](/help/adobe-support-tools-guide/assets/add-an-organization-1.png) toe
3. Specificeer a **naam** en het **land** van de organisatie.\
   De eenvoudige naam van de organisatie moet tussen 4 en 100 karakters zijn; maximumlengte voor pathname is 255 karakters.
   ![&#x200B; voeg kindOrganisatie &#x200B;](/help/adobe-support-tools-guide/assets/add-an-child-organization.png) toe
4. Selecteer **[!UICONTROL Save]**.
5. Selecteer **[!UICONTROL Review Pending Changes]** nadat u klaar bent met het bewerken van de organisaties. Na het herzien, uitgezocht **[!UICONTROL Submit Changes]** om [&#x200B; uit te voeren &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/execute-jobs.html) hen.

## Een onderliggende organisatie verwijderen

Als a [&#x200B; globale beheerder &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/manage-administrators.html), kunt u kindorganisaties schrappen. De verwijderingsbewerking kan niet ongedaan worden gemaakt en de basisorganisatie kan niet worden verwijderd. De middelen die aan de geschrapte organisatie worden toegewezen worden teruggegeven aan zijn ouderorganisatie. Voordat een organisatie wordt verwijderd, wordt het bovenliggende element automatisch de bovenliggende instantie van een van de onderliggende organisaties.

Een organisatie kan alleen worden geschrapt als aan de volgende criteria is voldaan:

- Er zijn geen Sign accounts, Adobe Stock-aankopen of opslagruimten in de organisatie.
- Er zijn geen geclaimde domeinen in de organisatie.
- Er zijn geen geïnstantieerde producten in de organisatie.
- Er zijn geen Experience Cloud-producten die instantiaties in de organisatie kunnen bevatten.

>[!WARNING]
>
>Het verwijderen van een organisatie heeft gevolgen voor uw gebruikers. Zorg ervoor dat er geen toegang of informatie is die verloren zal gaan wanneer een organisatie wordt geschrapt.

1. Meld u aan bij [[!DNL Global Admin Console] &#x200B;](https://global-admin-console.adobe.com/) . Ga naar het tabblad **[!UICONTROL Organizations]** en selecteer de organisatie die u wilt verwijderen.
1. Selecteer het pictogram **[!UICONTROL Delete]**.
   ![&#x200B; organisatie van de Schrapping &#x200B;](/help/adobe-support-tools-guide/assets/delete-organization.png)
1. Selecteer **[!UICONTROL Delete Organization]** in het dialoogvenster **[!UICONTROL OK]** .
1. Selecteer **[!UICONTROL Review Pending Changes]** nadat u klaar bent met het bewerken van de organisaties. Na het herzien, uitgezocht **[!UICONTROL Submit Changes]** om [&#x200B; uit te voeren &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/execute-jobs.html) hen.

## De naam van een organisatie wijzigen

De naam van de organisatie is de officiële naam van uw bedrijf of instelling, die tijdens de aankoop is ingesteld. Gebruikers zien deze naam wanneer ze een profiel selecteren tijdens hun aanmelding, vooral als ze toegang hebben tot Adobe-producten van meerdere organisaties of een keuze moeten maken tussen een zakelijk en een persoonlijk profiel.

Als a [&#x200B; globale beheerder &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/manage-administrators.html), kunt u de naam van om het even welke ouder of kindorganisatie uitgeven om gebruikers te helpen het correcte profiel identificeren wanneer het ondertekenen binnen aan [ [!DNL Creative Cloud]] producten en de diensten.

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/). Selecteer op het tabblad **[!UICONTROL Organizations]** de organisatie waarvan u de naam wilt wijzigen.
1. Selecteer het pictogram **[!UICONTROL Edit]**.
   ![&#x200B; noem organisatie &#x200B;](/help/adobe-support-tools-guide/assets/rename-organization.png) anders
1. Werk de naam van uw organisatie bij en selecteer **[!UICONTROL Save]** .

>[!TIP]
>
>Gebruik een duidelijke, herkenbare organisatienaam van maximaal 255 tekens om gebruikers te helpen het juiste profiel te selecteren. Vermijd het gebruik van speciale tekens en denk na over het opnemen van regio, afdeling of machtiging. Vermijd ook ongewone acroniemen en vage of vergelijkbare namen in de hiërarchie van uw organisatie.
>Gebruik een duidelijke, herkenbare organisatienaam tot 255 karakters om gebruikers te helpen het correcte profiel selecteren. Vermijd het gebruik van speciale tekens en denk na over het opnemen van regio, afdeling of machtiging. Ook, vermijd ongewone acroniemen en vage of gelijkaardige namen over uw organisatiehiërarchie.

Wijzigingen worden vastgelegd in het auditlogbestand, alle gebruikers worden via e-mail op de hoogte gesteld en de naam kan niet 24 uur lang opnieuw worden bijgewerkt. [&#x200B; Leer om controlelogboeken &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/insights.html) te bekijken en te downloaden.

## Het bovenliggende element van een organisatie wijzigen

Als [[!DNL Global Administrator]](https://helpx.adobe.com/enterprise/global-admin-console/manage-administrators.html) kunt u een organisatie in de organisatiehiërarchie weergeven met de knop **[!UICONTROL Change hierarchy]** .

Het wijzigen van het bovenliggende element van een organisatie heeft de volgende gevolgen:

- Als een organisatie wordt geparseerd, wordt de volledige subboomstructuur met de bovenliggende organisatie mee verplaatst. De padnamen van de gerepareerde organisatie en de bijbehorende kinderen worden bijgewerkt met de nieuwe locatie ervan.
- Het beleid van de organisatie [&#x200B; &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/update-policies.html) van verplaatste organisaties wordt bijgewerkt zodat om het even welke sloten op beleid door een organisatie in de nieuwe hiërarchie worden gehouden.
- Als u de positie van een organisatie in de hiërarchie wijzigt, kunnen de algemene beheerders voor die organisatie worden gewijzigd. Algemene beheerrollen worden in de hiërarchie overgeërfd, zodat alle algemene beheerders van de nieuwe bovenliggende organisatie automatisch globale beheerders van de verplaatste organisatie worden. Evenzo kunnen globale beheerders hun rol in de verplaatste organisatie verliezen als zij die rol hadden omdat zij een globale beheerder van de oude ouder waren. De overgeërfde algemene beheerrollen worden niet vermeld in het deelvenster Beheerders van de organisatie.
- Het onderbrengen beïnvloedt ook de beschikbare producten in de verplaatste organisaties. Wanneer mogelijk, [&#x200B; producttoewijzingen &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/allocate-products.html) worden bijgewerkt zodat komen zij via de nieuwe ouderplaats.
- Als de producttoewijzingen niet kunnen worden bijgewerkt om van de nieuwe ouder te komen, worden de producten samen met de productprofielen van die producten verwijderd. Deze bewerking kan ertoe leiden dat gebruikers de toegang verliezen. Het product is alleen beschikbaar op de nieuwe locatie als de meest gangbare voorouder van de oude en nieuwe locaties over het product beschikt.

>[!WARNING]
>
>Als producten worden verwijderd als gevolg van reparatie, verliezen gebruikers de toegang tot die producten.

1. Teken binnen aan de [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/). Selecteer op het tabblad **[!UICONTROL Organizations]** de optie **[!UICONTROL Change hierarchy]** om het opnieuw instellen van organisaties in te schakelen.
2. Selecteer **[!UICONTROL &#x200B; OK]** in het pop-upscherm dat verschijnt.
3. Sleep de onderliggende organisatie boven aan de gewenste organisatie om deze te reparent.
4. Selecteer **[!UICONTROL Save]** wanneer u klaar bent met het repareren van uw organisaties.
5. Selecteer **[!UICONTROL Review Pending Changes]** nadat u klaar bent met het bewerken van de organisaties. Na het herzien, selecteer **[!UICONTROL Submit Changes]** om [&#x200B; &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/execute-jobs.html) hen uit te voeren.

Zodra de baan volledig is, kunt u aan de Toewijzing van het Product en [&#x200B; verandering de subsidiewaarden &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/allocate-products.html) navigeren om op de verandering in toewijzing van productmiddelen te wijzen.

## Bestaande organisaties toevoegen met de Organizer Mapper

Als a [&#x200B; Globale Beheerder &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/manage-administrators.html), kunt u bestaande organisaties toevoegen die momenteel geen deel van uw hiërarchie van de Global Admin Console aan de organisatiehiërarchie zijn.

U kunt ook teamorganisaties toevoegen aan de organisatiehiërarchie. Teamorganisaties nemen niet deel aan producttoewijzing of productgebruiksllup, en het beheer van teamorganisaties in de Global Admin Console is beperkt. U kunt ze toevoegen aan de organisatiehiërarchie om ze bij te houden en de producten die ze kopen zichtbaar te maken. Teamorganisaties kunnen geen onderliggende organisaties onder hen hebben en hebben niet veel van de eigenschappen van ondernemingsorganisaties.

Leer meer over de [&#x200B; beperkingen op producttoewijzing &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/allocate-products.html#limitations).

>[!WARNING]
>
> U kunt alleen onderliggende organisaties toevoegen aan basisorganisaties die op hetzelfde opslagmodel zijn gebaseerd. Zo, kunnen de kindorganisaties die op het model van de gebruikersopslag worden gebaseerd slechts aan wortelorganisaties worden toegevoegd die op het model van de gebruikersopslag worden gebaseerd. En onderliggende organisaties die zijn gebaseerd op het opslagmodel voor bedrijven kunnen alleen worden toegevoegd aan basisorganisaties die zijn gebaseerd op het opslagmodel voor bedrijven.
>U kunt alleen onderliggende organisaties toevoegen aan basisorganisaties die op hetzelfde opslagmodel zijn gebaseerd. Zo, kunnen de kindorganisaties die op het model van de gebruikersopslag worden gebaseerd slechts aan wortelorganisaties worden toegevoegd die op het model van de gebruikersopslag worden gebaseerd. En onderliggende organisaties die zijn gebaseerd op het opslagmodel voor bedrijven kunnen alleen worden toegevoegd aan basisorganisaties die zijn gebaseerd op het opslagmodel voor bedrijven.

Het tabblad **[!UICONTROL Organization Mapper]** geeft het volgende weer:

1. Een vervolgkeuzelijst met een lijst met mogelijke bovenliggende organisaties waaraan u een onderliggende organisatie kunt toevoegen. Dit zijn organisaties waarvoor u een globale beheerder bent.
1. Een lijst met onderliggende organisaties die kunnen worden toegevoegd onder het bovenliggende element dat is geselecteerd in stap 1. Dit zijn organisaties waarvoor u een systeembeheerder bent en die nog geen kind van een andere organisatie zijn.

Wanneer een organisatie aan globaal beleid wordt toegevoegd, blijven de producten in de organisaties die gebruikend de mapper van de Organisatie worden toegevoegd als aankopen; [&#x200B; de aantallen van de Toewijzing van het 0&rbrace; Product houden rollup bij deze organisaties.](https://helpx.adobe.com/enterprise/global-admin-console/allocate-products.html)

1. Teken binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/), en navigeer aan **[!UICONTROL Organization Mapper]**.
2. Selecteer een bovenliggende organisatie in de vervolgkeuzelijst.\
   Dit zijn de organisaties waarvoor u direct als globale beheerder wordt toegevoegd. Als u in de vervolgkeuzelijst geen organisatie ziet die u als bovenliggend element wilt gebruiken, selecteert u een hogere organisatie in de hiërarchie. Zodra de Organisatie mapper verrichting volledig is, kunt u [&#x200B; hiërarchie van de Verandering &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/set-up-organizations.html#change-the-parent-of-an-organization) gebruiken om de nieuwe organisatie neer in de boom te bewegen om de ouder te hebben u wilt gebruiken.
3. Selecteer de organisaties die als onderliggende organisaties van de in de vorige stap geselecteerde organisatie moeten worden toegevoegd.
4. Selecteer **[!UICONTROL Review Pending Changes]**. Dan, selecteer **[!UICONTROL Submit Changes]** om [&#x200B; uit te voeren &#x200B;](https://helpx.adobe.com/enterprise/global-admin-console/execute-jobs.html) hen.
5. Nadat u de wijzigingen hebt uitgevoerd, kunt u de bovenstaande stappen herhalen om extra onderliggende organisaties toe te voegen aan de hiërarchie van uw organisatie.

Als een organisatie zich in de hiërarchie bevindt, kunt u het organisatiebeleid, de beheerders of andere instellingen aanpassen door naar het tabblad **[!UICONTROL Organizations]** te navigeren.
