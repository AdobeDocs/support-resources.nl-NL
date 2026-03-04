---
title: Kan gebruiker niet toevoegen aan Adobe Commerce Cloud Project
description: Dit artikel biedt een oplossing als u geen gebruiker kunt toevoegen aan een Adobe Commerce-cloudproject.
feature: Cloud, Paas
solution: Commerce
feature-set: Commerce
role: Developer
exl-id: 2dc52d5e-0930-48c4-986e-ce3f9f6f8221
source-git-commit: 755c6dc9cff041b9ca9183fbecde21f90fbaee1a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Kan gebruiker niet toevoegen aan Adobe Commerce Cloud Project

Dit artikel verstrekt een oplossing voor wanneer u probeert om een gebruiker aan een wolkenproject toe te voegen, maar het ontbreekt met een fout: *Gebruiker XXX bestaat niet*.

## Betrokken producten en versies

* Adobe Commerce op wolkeninfrastructuur, [ alle gesteunde versies ](https://magento.com/sites/default/files/magento-software-lifecycle-policy.pdf)

## Probleem

Dit artikel biedt een oplossing als u geen gebruiker kunt toevoegen aan een Adobe Commerce-cloudproject.

## Oorzaak

De rekening van de gebruiker moet eerst in [ https://accounts.magento.cloud ](https://accounts.magento.cloud) worden gecreeerd en met hun Adobe SSO verbonden alvorens zij als gebruiker aan het project kunnen worden toegevoegd. Als de gebruiker een Adobe-account maar geen Commerce (magento.com) account heeft, moet hij of zij eerst een account maken.

## Oplossing

1. Vraag de gebruiker om binnen bij [ https://accounts.magento.cloud ](https://accounts.magento.cloud) te ondertekenen. De gebruiker moet al bij Adobe zijn geregistreerd met hetzelfde e-mailadres.
   >[!NOTE]
   >Het creëren van of het hebben van een rekening in [ https://account.adobe.com ](https://account.adobe.com) betekent niet automatisch dat de gebruiker een rekening in [ https://accounts.magento.cloud ](https://accounts.magento.cloud) heeft. De gebruiker moet eerst [ tot hun rekening van Commerce ](https://experienceleague.adobe.com/en/docs/commerce-admin/start/commerce-account/commerce-account-create?lang=en#create-a-commerce-account) leiden.

1. Als de gebruiker reeds een rekening van Adobe heeft maar niet kan binnen ondertekenen, hen vragen om a [ steunverzoek ](https://experienceleague.adobe.com/home#support) met [!UICONTROL Issue Reason] voor te leggen geplaatst aan *Gebruikersbeheer*.

1. Nadat de gebruiker met succes binnen aan [ https://accounts.magento.cloud ](https://accounts.magento.cloud) ondertekent, kunt u de gebruiker aan het project toevoegen. Voor gedetailleerde stappen, zie [ gebruikers toevoegen en toegang ](https://experienceleague.adobe.com/en/docs/commerce-cloud-service/user-guide/project/user-access#add-users-and-manage-access) in Commerce op de Gids van de Infrastructuur van de Wolk beheren.

## Gerelateerde lezing:

* [ beheer gebruikerstoegang ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) in onze Commerce op de Gids van de Infrastructuur van de Wolk.
* [ Onbekwaam aan login aan de steun van Adobe Commerce of wolkenrekening ](https://experienceleague.adobe.com/docs/commerce-knowledge-base/kb/troubleshooting/miscellaneous/unable-to-log-in-to-support-or-cloud-project.html)
