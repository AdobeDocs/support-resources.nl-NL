---
title: Adobe-configuratie voor klantenondersteuning
description: Hoe Adobe-klanten supportrechten kunnen configureren om caseverzending mogelijk te maken.
feature-set: Experience Cloud Services
solution: Admin Console
feature: Admin Console
source-git-commit: 009be3353a4bd690a7cf395e7e95540808058b39
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# Adobe-machtiging voor klantenondersteuning

Als u supportrechten voor uw organisatie wilt configureren, moet u eerst de gebruiker via de Admin Console toevoegen of uitnodigen.

## Ondersteuningsmachtigingsrollen toevoegen aan een organisatie

De rol van steunbeheerder is een niet administratieve rol die toegang tot steun-verwante informatie heeft. Ondersteuningsbeheerders kunnen probleemrapporten weergeven, maken en beheren.

Een beheerder toevoegen of uitnodigen:

1. Kies in de Admin Console **[!UICONTROL Users]** > **[!UICONTROL Administrators]** .
1. Klik op **[!UICONTROL Add Admin]**.
1. Voer een naam of e-mailadres in.

   U kunt zoeken naar bestaande gebruikers of een nieuwe gebruiker toevoegen door een geldig e-mailadres op te geven en de gegevens op het scherm in te vullen.

   ![ voeg admin ](assets/admin-console-add-admin.png) toe

1. Klik op **[!UICONTROL Next]**. Er wordt een lijst met beheerrollen weergegeven.

Om een rol van Admin van de Steun aan een gebruiker toe te wijzen (laat een gebruiker toe om steun te kunnen contacteren):

1. Selecteer de optie **[!UICONTROL Support administrator]** .

   ![ geef admin rechten ](assets/edit-admin-rights.png) uit

1. Kies een van de volgende twee opties:

   * Optie 1: **[!UICONTROL Basic support administrator]**. Selecteer deze optie als u de gebruikersondersteuning toegang wilt geven tot alle oplossingen (behalve Marketo Engage).
   * Optie 2: **[!UICONTROL Product support administrator]**: selecteer deze optie voor Marketo Engage-ondersteuning. Selecteer welke Marketo Engage-instanties de gebruiker toegang geven.

   ![ geef admin rechten Marketo ](assets/edit-admin-rights-advanced.png) uit

1. Als u de selecties hebt aangebracht, klikt u op **[!UICONTROL Save]** .

De gebruiker ontvangt een e-mailuitnodiging met betrekking tot de nieuwe beheerrechten van `message@adobe.com` .

Gebruikers moeten in de e-mail op **[!UICONTROL Get started]** klikken om lid te worden van de organisatie. Als nieuwe beheerders de koppeling **[!UICONTROL Get started]** niet gebruiken in de e-mailuitnodiging, kunnen ze zich niet aanmelden bij de Admin Console.

Als onderdeel van het aanmeldingsproces kunnen gebruikers worden gevraagd een Adobe-profiel in te stellen als ze dat nog niet hebben. Als gebruikers meerdere profielen hebben gekoppeld aan hun e-mailadres, moeten gebruikers **[!UICONTROL Join Team]** kiezen (indien gevraagd) en vervolgens het profiel selecteren dat is gekoppeld aan de nieuwe organisatie.

![ Bevestiging van Admin-rechten ](assets/admin-rights-confirmation.png)

Voor meer details verwijs naar [ uitgeeft onderneming admin rolinstructies ](admin-roles.md#add-enterprise-role) in de administratieve roldocumentatie. Merk op dat slechts een systeembeheerder voor uw organisatie deze rol kan toewijzen. Voor meer informatie over administratieve hiërarchie, bezoek de [ administratieve rollen ](admin-roles.md) documentatie.
