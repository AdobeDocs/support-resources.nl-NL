---
title: Licentietoewijzingsrapporten maken voor meerdere organisaties en producten
description: U kunt rapporten met licentietoewijzingen genereren, weergeven en downloaden voor meerdere organisaties en producten in de Global Admin Console.
Feature-set: Experience Cloud Services
Solution: Admin Console
Feature: Admin Console
exl-id: e3380a89-8529-473f-bd17-efb05466eab9
source-git-commit: dbbd971e57265e1651f44f834e56d461159ab4fc
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Licentietoewijzingsrapporten maken voor meerdere organisaties en producten

Leer hoe globale beheerders gedetailleerde licentierapporten voor meerdere organisaties en producten voor specifieke datumbereiken kunnen genereren en downloaden om het nauwkeurig bijhouden van licentieverlening te vergemakkelijken.

>[!NOTE]
>
>Om, een rapport van de vergunningstaak tot stand te brengen te bekijken en uit te voeren, binnen aan [&#x200B; Global Admin Console &#x200B;](https://global-admin-console.adobe.com/) te ondertekenen, en naar **[!UICONTROL Insights]** te gaan > **[!UICONTROL Reports]** > **[!UICONTROL License assignment]**.

## Een rapport maken

Met licentietoewijzingsrapporten kunt u de provisioning van licenties proactief controleren en handmatige tracering verminderen. Globale beheerders kunnen een licentietoewijzingsrapport maken voor bepaalde producten voor een willekeurig aantal onderliggende organisaties om de gegevens over de levering van softwarelicenties op alle afdelingen te controleren.

1. Ga naar het **[[!UICONTROL Insights]](https://global-admin-console.adobe.com/insights)** lusje in Global Admin Console.
1. Selecteer op de pagina **[!UICONTROL License Assignment]** de optie **[!UICONTROL Create report]** .
1. Selecteer de organisaties en selecteer **[!UICONTROL Next]** . U kunt elke organisatie afzonderlijk kiezen of alle onderliggende organen binnen een bovenliggende instantie selecteren met de knop **[!UICONTROL Select all]** .

>[!NOTE]
>
>**weet waarom u bepaalde organisaties** niet kunt selecteren:
>Als een onderliggende org geen contract heeft of een afzonderlijk ondernemingscontract heeft met hetzelfde product als dat van de bovenliggende org, is deze uitgeschakeld voor het maken van een licentietoewijzingsrapport. Als het contract van de bovenliggende org bijvoorbeeld Adobe Acrobat heeft en de onderliggende org hetzelfde heeft als een onderdeel van een ander contract, is het product beperkt voor toewijzing. Hierdoor is het ook beperkt voor het maken van rapporten in de Global Admin Console. [&#x200B; Leer hoe te om levering voor dergelijke organisaties te volgen gebruikend hun respectieve Admin Console &#x200B;](https://helpx.adobe.com/nl/enterprise/using/assignment-reports.html).
>
>[!NOTE]
>
>U kunt toewijzingsrapporten alleen maken voor organisaties met een actief contract.

1. Selecteer de producten die u in het rapport wilt opnemen en selecteer **[!UICONTROL Next]** .

>[!NOTE]
>
>**weet waarom u bepaalde producten** niet kunt selecteren:
>Producten die niet kunnen worden toegewezen in de Global Admin Console, worden niet opgenomen voor het maken van rapporten. Dit omvat momenteel enkele Digital Experience-producten zoals [!DNL Workfront] , [!DNL Adobe Experience Manager] en [!DNL Adobe Experience Platform] , en ook producten zoals [!DNL Adobe Firefly Services] , [!DNL Acrobat Sign] en [!DNL Adobe Stock] . [&#x200B; u gebruikt Adobe Admin Console om de gegevens van de vergunningslevering voor deze producten &#x200B;](https://helpx.adobe.com/nl/enterprise/using/assignment-reports.html) te vinden.

1. Selecteer of het rapport per maand of jaar moet worden samengevoegd.
1. Selecteer een aangepast datumbereik of kies een van de vooraf ingestelde opties. U kunt elke begindatum kiezen van 18 juni 2020 tot en met de vorige dag, zolang deze niet voorafgaat aan de begindatum van uw contract.
1. Selecteer **[!UICONTROL Download]** om het rapport als CSV-bestand te exporteren.

Het rapport begint met de verwerking en verschijnt op de **[!UICONTROL License Assignment]** -pagina met details zoals naam, maker, aanmaaktijd, datumbereik en status. Zodra u klaar bent, ontvangt u een e-mailbericht en wordt het rapport automatisch gedownload.

Om het even welke globale admin kan het rapport op om het even welk ogenblik downloaden nadat het klaar is, gebruikend het **[!UICONTROL Download]** pictogram naast de rapportnaam.

>[!NOTE]
>
>- Om ervoor te zorgen dat de meest recente gegevens worden weergegeven, genereert u rapporten 48 uur na elke toewijzing.
>- Rapporten worden 90 dagen bewaard nadat ze zijn gegenereerd.

## Eerder gegenereerde rapporten weergeven en downloaden

Globale beheerders kunnen de rapporten van de vergunningstoewijzing bekijken en downloaden die door andere globale admin in uw organisatie worden geproduceerd. Globale viewers kunnen echter alleen de lijst met licentietoewijzingsrapporten weergeven.

1. Ga naar het **[[!UICONTROL Insights]](https://global-admin-console.adobe.com/insights)** lusje in Global Admin Console.
1. Op de pagina **[!UICONTROL License Assignment]** worden alle rapporten weergegeven met de volgende details:

   | Veld | Beschrijving |
   | ------------- | ------------------------------------------------------------------------------------------------- |
   | Naam | Automatisch gegenereerd en kan niet worden bewerkt. |
   | Maker | De algemene beheerder die het rapport heeft gegenereerd. |
   | Aanmaaktijd | De systeemtijd toen het rapport werd gecreeerd. |
   | Datumbereik | Het geselecteerde datumbereik voor het rapport. |
   | Status | **Succes** als het rapport klaar voor download is, of **Verwerking** als het nog wordt geproduceerd. |

1. Als u het rapport wilt exporteren als een CSV-bestand, selecteert u het pictogram **[!UICONTROL Download]** naast het rapport.

## Kennis van uw licentietoewijzingsrapport

Het rapport dat u downloadt, bevat de volgende informatie voor elke gebeurtenis:

| Veld | Beschrijving |
| -------------------------------- | -------------------------------------------------------- |
| Org-id | Unieke id gekoppeld aan de bovenliggende org |
| Org name | Naam van de bovenliggende org |
| Child org ID | Unieke id van de geselecteerde onderliggende org |
| Naam van onderliggende org | Naam van de onderliggende org |
| Licentie-id | Unieke id voor de productlicentie |
| Productnaam | Naam van het geselecteerde product |
| Datum | Datumselectie |
| Totale hoeveelheid vergunning | Totaal aantal licenties op het niveau van de bovenliggende org |
| Kinderlicenties | Licentietelling die wordt toegewezen aan de onderliggende org |
| Toegewezen hoeveelheid maandelijks/jaarlijks piek | Geaggregeerde waarde van de licentieverlening (maandelijks/jaarlijks) |
