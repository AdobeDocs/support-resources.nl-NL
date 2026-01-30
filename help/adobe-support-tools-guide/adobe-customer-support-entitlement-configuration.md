---
title: Adobe-configuratie voor klantenondersteuning
description: Hoe Adobe-klanten supportrechten in de Admin Console kunnen instellen en beheren, zodat gebruikers toegang hebben tot ondersteuningsbronnen, problemen kunnen indienen en de activiteiten van de kwestie kunnen beheren.
feature-set: Experience Cloud Services
solution: Admin Console
feature: Admin Console
source-git-commit: 7f7a394874014fb5333ed9fb39f84b7137562726
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Adobe-configuratie voor klantenondersteuning

Als u supportrechten voor uw organisatie wilt configureren, moet u eerst de gebruiker via de Admin Console toevoegen of uitnodigen.

## Ondersteuningsmachtigingsrollen toevoegen aan een organisatie

De rol **[!UICONTROL Support administrator]** is een niet-administratieve rol die toegang tot steun-verwante informatie heeft. Een **[!UICONTROL Support administrator]** kan probleemrapporten weergeven, maken en beheren.

Een beheerder toevoegen of uitnodigen:

1. Kies in de Admin Console **[!UICONTROL Users]** > **[!UICONTROL Administrators]** .
1. Klik op **[!UICONTROL Add Admin]**.
1. Voer een naam of e-mailadres in.

   U kunt zoeken naar bestaande gebruikers of een nieuwe gebruiker toevoegen door een geldig e-mailadres op te geven en de gegevens op het scherm in te vullen.

   ![&#x200B; voeg admin &#x200B;](assets/admin-console-add-admin.png) toe

1. Klik op **[!UICONTROL Next]**. Er wordt een lijst met beheerrollen weergegeven.

Een **[!UICONTROL Support administrator]** -rol toewijzen aan een gebruiker (een gebruiker inschakelen om contact op te nemen met ondersteuning):

1. Selecteer de optie **[!UICONTROL Support administrator]** .

   ![&#x200B; geef admin rechten &#x200B;](assets/edit-admin-rights.png) uit

1. Kies een van de volgende twee opties:

   * Optie 1: **[!UICONTROL Basic support administrator]**. Selecteer deze optie als u de gebruikersondersteuning toegang wilt geven tot alle oplossingen (behalve Marketo Engage).
   * Optie 2: **[!UICONTROL Product support administrator]**: selecteer deze optie voor Marketo Engage-ondersteuning. Selecteer welke Marketo Engage-instanties de gebruiker toegang geven.

   ![&#x200B; geef admin rechten Marketo &#x200B;](assets/edit-admin-rights-advanced.png) uit

1. Als u de selecties hebt aangebracht, klikt u op **[!UICONTROL Save]** .

De gebruiker ontvangt een e-mailuitnodiging met betrekking tot de nieuwe beheerrechten van `message@adobe.com` .

Gebruikers moeten in de e-mail op **[!UICONTROL Get started]** klikken om lid te worden van de organisatie. Als nieuwe beheerders de koppeling **[!UICONTROL Get started]** niet gebruiken in de e-mailuitnodiging, kunnen ze zich niet aanmelden bij de Admin Console.

Als onderdeel van het aanmeldingsproces kunnen gebruikers worden gevraagd een Adobe-profiel in te stellen als ze dat nog niet hebben. Als gebruikers meerdere profielen hebben gekoppeld aan hun e-mailadres, moeten gebruikers **[!UICONTROL Join Team]** kiezen (indien gevraagd) en vervolgens het profiel selecteren dat is gekoppeld aan de nieuwe organisatie.

![&#x200B; Bevestiging van Admin-rechten &#x200B;](assets/admin-rights-confirmation.png)

Voor meer details verwijs naar [&#x200B; uitgeeft onderneming admin rolinstructies &#x200B;](admin-roles.md#edit-enterprise-admin-role) in de administratieve roldocumentatie. Merk op dat slechts een systeembeheerder voor uw organisatie deze rol kan toewijzen. Voor meer informatie over administratieve hiërarchie, bezoek de [&#x200B; Administratieve rollen &#x200B;](admin-roles.md) documentatie.
