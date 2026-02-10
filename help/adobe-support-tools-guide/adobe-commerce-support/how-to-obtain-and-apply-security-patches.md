---
title: Procedure voor ophalen en toepassen [!UICONTROL security patch]
description: Dit artikel bevat instructies voor het ophalen en toepassen van een vrijgegeven [!UICONTROL security patch] , maar instructies zijn niet beschikbaar.
source-git-commit: 93ee9bd110930e244befca682fadd3edc24d138a
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Een [!UICONTROL security patch] ophalen en toepassen

>[!NOTE]
>Als u een installatie op locatie hebt en geen versiecontrolesystemen zoals [!DNL CVS] of GitHub gebruikt om uw code te beheren, zou uw Webgastheer met het toepassen van het flard kunnen kunnen helpen. Voel je vrij om hen te bereiken voor steun.

Dit artikel bevat instructies voor het ophalen en toepassen van een vrijgegeven [!UICONTROL security patch] , maar instructies zijn niet beschikbaar.

## Betrokken producten en versies

Adobe Commerce on-premise en cloud-infrastructuur - alle ondersteunde versies


## Oorzaak

De meeste [!UICONTROL security patches] worden vrijgegeven zonder afzonderlijke patch of hotfix en moeten worden bijgewerkt naar de release van [!UICONTROL security patch] .

## Oplossing


### Zaak I:

* Als een geïsoleerd flarddossier/hotfix in de [&#x200B; Nota&#39;s van de Versie &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-on-cloud/user-guide/release-notes/cloud-tools-suite) wordt vermeld, download het dossier van de downloadsectie van [&#x200B; https://account.magento.com &#x200B;](https://account.magento.com/downloads/view/). Gebruikers met gedeelde toegang moeten eerst downloadrechten krijgen van de eigenaar/licentiehouder van de account.

**beveats:**

Als u op een oudere versie van Adobe Commerce (2.4.4) werkt, hebt u automatisch Extended Support ontvangen. Uw versie moet een van de volgende niet-ondersteunde versies zijn om de nieuwste beschikbare beveiligingspatches toe te passen:

2.4.4 - 2.4.4-p11

Niet-ondersteunde versies (2.3.x, 2.4.0 - 2.4.3) komen niet in aanmerking voor ondersteuning en u moet eerst een upgrade uitvoeren naar een ondersteunde versie om te profiteren van de meest recente beveiligingsoplossingen.

Als u geen uitgebreide ondersteuning hebt, kunt u ondersteuning vragen om de patches met u te delen, maar deze kunnen geen problemen/fouten oplossen die u bij het toepassen van de patches kunt tegenkomen.

### Zaak II:

De geïsoleerde flarden worden slechts verstrekt in uitzonderlijke gevallen, en het is niet de aangewezen vorm om veiligheidsmoeilijke situaties uit te voeren.

Als een afzonderlijk patchbestand/hotfix niet wordt vermeld in de opmerkingen bij de release:

* **Wolk:**

1. Sommige [!UICONTROL security patches] zouden in de recentste versie van de Reeks van Hulpmiddelen van de Wolk (ECE Hulpmiddelen) onder de Patches van de Wolk voor Commerce kunnen worden omvat/worden vrijgegeven - controleer de [&#x200B; Nota&#39;s van de Versie &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-cloud-service/user-guide/release-notes/cloud-tools-suite), en als een veiligheidsmoeilijke situatie in de versie wordt vermeld, bevorder het pakket aan die versie.
1. Als in de opmerkingen bij de release geen melding wordt gemaakt van een beveiligingscorrectie, gaat u verder met lezen.

* **de infrastructuur van de Wolk of op-Premise:**

* Als een geïsoleerd flarddossier/hotfix niet beschikbaar is, [&#x200B; bevorder de versie van Adobe Commerce op wolkeninfrastructuur &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-cloud-service/user-guide/develop/upgrade/commerce-version) 2.4.X aan recentste flardversie 2.4.X-pY.
* Als een geïsoleerd flarddossier/hotfix niet beschikbaar is, [&#x200B; bevorder de versie van Adobe Commerce On-Premise &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-operations/upgrade-guide/implementation/perform-upgrade) 2.4.X aan recentste flardversie 2.4.X-pY.

## Gerelateerde lezing

* Zie [&#x200B; de nota&#39;s van de Versie voor de Reeks van Commerce Cloud Tools &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-cloud-service/user-guide/release-notes/cloud-tools-suite) in *Adobe Commerce op de Gids van de Infrastructuur van de Wolk*.
* Zie [&#x200B; de versie van Adobe Commerce &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-cloud-service/user-guide/develop/upgrade/commerce-version) in *Adobe Commerce op de Gids van de Infrastructuur van de Wolk* bevorderen.
