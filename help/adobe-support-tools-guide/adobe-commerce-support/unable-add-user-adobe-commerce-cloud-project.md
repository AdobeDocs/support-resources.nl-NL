---
title: Kan gebruiker niet toevoegen aan Adobe Commerce Cloud Project
description: Dit artikel biedt een oplossing als u geen gebruiker kunt toevoegen aan een Adobe Commerce-cloudproject.
feature: Cloud, Paas
solution: Commerce
feature-set: Commerce
role: Developer
source-git-commit: dfb3e7ea8638755cdff16b0765125403f429ef2e
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# Kan gebruiker niet toevoegen aan Adobe Commerce Cloud Project

Dit artikel verstrekt een oplossing voor wanneer u probeert om een gebruiker aan een wolkenproject toe te voegen, maar het ontbreekt met een fout: *Gebruiker XXX bestaat niet*.

## Betrokken producten en versies

* Adobe Commerce op wolkeninfrastructuur, [&#x200B; alle gesteunde versies &#x200B;](https://magento.com/sites/default/files/magento-software-lifecycle-policy.pdf)

## Probleem

Dit artikel biedt een oplossing als u geen gebruiker kunt toevoegen aan een Adobe Commerce-cloudproject.

## Oorzaak

De rekening van de gebruiker moet eerst in [&#x200B; https://accounts.magento.cloud &#x200B;](https://accounts.magento.cloud) worden gecreeerd en met hun Adobe SSO verbonden alvorens zij als gebruiker aan het project kunnen worden toegevoegd. Als de gebruiker een Adobe-account maar geen Commerce (magento.com) account heeft, moet hij of zij eerst een account maken.

## Oplossing

1. Vraag de gebruiker om binnen bij [&#x200B; https://accounts.magento.cloud &#x200B;](https://accounts.magento.cloud) te ondertekenen. De gebruiker moet al bij Adobe zijn geregistreerd met hetzelfde e-mailadres.
   > **OPMERKING**\
   > Het creëren van of het hebben van een rekening in [&#x200B; https://account.adobe.com &#x200B;](https://account.adobe.com) betekent niet automatisch dat de gebruiker een rekening in [&#x200B; https://accounts.magento.cloud &#x200B;](https://accounts.magento.cloud) heeft. De gebruiker moet eerst [&#x200B; tot hun rekening van Commerce &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-admin/start/commerce-account/commerce-account-create?lang=en#create-a-commerce-account) leiden.

1. Als de gebruiker reeds een rekening van Adobe heeft maar niet kan binnen ondertekenen, hen vragen om a [&#x200B; steunverzoek &#x200B;](https://experienceleague.adobe.com/home?lang=nl-NL#support) met [!UICONTROL Issue Reason] voor te leggen geplaatst aan *Gebruikersbeheer*.

1. Nadat de gebruiker met succes binnen aan [&#x200B; https://accounts.magento.cloud &#x200B;](https://accounts.magento.cloud) ondertekent, kunt u de gebruiker aan het project toevoegen. Voor gedetailleerde stappen, zie [&#x200B; gebruikers toevoegen en toegang &#x200B;](https://experienceleague.adobe.com/nl/docs/commerce-cloud-service/user-guide/project/user-access#add-users-and-manage-access) in Commerce op de Gids van de Infrastructuur van de Wolk beheren.

## Gerelateerde lezing:

* [&#x200B; beheer gebruikerstoegang &#x200B;](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html?lang=nl-NL) in onze Commerce op de Gids van de Infrastructuur van de Wolk.
* [&#x200B; Onbekwaam aan login aan de steun van Adobe Commerce of wolkenrekening &#x200B;](https://experienceleague.adobe.com/docs/commerce-knowledge-base/kb/troubleshooting/miscellaneous/unable-to-log-in-to-support-or-cloud-project.html?lang=nl-NL)