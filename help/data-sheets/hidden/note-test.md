---
description: Verbinding maken met de Widget-Data Warehouse - Productdocumentatie
title: Verbinding maken met de Widget-Data Warehouse
hide: true
hidefromtoc: true
exl-id: d6a7cff5-08f9-4c93-8765-46e692feaa0d
source-git-commit: 972704990172c966a27744b49b9f7af5626e9f3e
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Verbinding maken met de Widget-Data Warehouse {#connecting-to-the-widget-data-warehouse}

## Nieuwe test

<ol><li>Gebruik de ` {{name}} ` variabele.</li></ol>

<ol><li>Gebruik &trace;&trace;<code>name</code>&break;&amp; &break; variable.</li></ol>

## Geneste test

**eerst**

>[!NOTE]
>
>U kunt het volgende niet verwijderen:
>
>* De ingebouwde statussen Planning, Huidig, en Volledig. U kunt hun namen bijwerken, hun kleuren bewerken en vergrendelen of ontgrendelen, maar ze kunnen niet worden verwijderd.
>* Statussen die in een goedkeuringsstatus verkeren voor ten minste één object in uw systeem.

**Second**

>[!NOTE]
>
>U kunt het volgende niet verwijderen:
>
>* De ingebouwde statussen Planning, Huidig, en Volledig. U kunt hun namen bijwerken, hun kleuren bewerken en vergrendelen of ontgrendelen, maar ze kunnen niet worden verwijderd.
>
>  Dit ligt tussen
>
>* Statussen die in een goedkeuringsstatus verkeren voor ten minste één object in uw systeem.

## Koppeling naar widget-toegang {#widget-access-link}

Als u toegang wilt krijgen tot uw Widget-gegevensopslagruimte, moet u naar de specifieke URL voor uw Widget-account navigeren.  U vindt deze toegangskoppeling door u aan te melden bij Marketo Measure en onderstaande stappen te volgen om naar de pagina met informatie over Data Warehouse te navigeren.

1. In Marketo Measure, bij de bovenkant van de pagina, klik **Mijn Rekening** > **Montages**.

   ![](assets/adobe-logo-old.png)

1. Op het linkerzijmenu, onder Veiligheid, klik **Data Warehouse**.

   ![](assets/adobe-logo-old.png)

1. Op deze pagina, zult u de verbinding aan uw het gegevenspakhuis van Widget en uw gebruikersbenaming vinden.

   ![](assets/adobe-logo-old.png)

   >[!NOTE]
   >
   >Dit is een alleen-lezen account dat beschikbaar is voor uw organisatie, en niet alleen voor een individuele gebruiker. Elke gebruiker binnen uw organisatie die toegang heeft tot Marketo Measure, kan dit account gebruiken om u aan te melden bij het account voor een widgetlezer.

1. Klik op de koppeling in de URL van de widget. Hiermee gaat u naar de aanmeldingspagina van de widget waarin u uw gebruikersnaam en wachtwoord kunt invoeren. _als u uw wachtwoord niet hebt, zie de stappen hieronder om het_ terug te stellen.

   ![](assets/adobe-logo-old.png)

1. Zodra het programma geopend, klik **Werkbladen** bij de bovenkant van de pagina.

   ![](assets/adobe-logo-old.png)

1. De BIZIBLE_ROI_V3-databaseobjecten bevinden zich aan de linkerkant van het scherm.  Ga het Warehouse, het Gegevensbestand, en het Schema van de dropdown opties bij de bovenkant van het vraagvenster in.  Er mag slechts één optie voor elke optie zijn.  Nu kunt u query&#39;s uitvoeren in de widget-query-editor.

   ![](assets/adobe-logo-old.png)

## Wachtwoord opnieuw instellen {#reset-your-password}

Marketo Measure heeft geen toegang tot uw wachtwoord voor widgetaanmelding.  Als u uw wachtwoord opnieuw moet instellen, klik de knoop van het Wachtwoord van het Terugstellen op de de informatiepagina van de Data Warehouse, en volg de instructies. Er wordt direct een tijdelijk wachtwoord weergegeven in de gebruikersinterface. U zal worden ertoe aangezet om uw eigen wachtwoord op uw volgende login van het gegevenspakhuis tot stand te brengen.

>[!NOTE]
>
>* Als u het wachtwoord opnieuw instelt, wordt dit opnieuw ingesteld voor alle Marketo Measure-gebruikers in uw organisatie, en niet alleen voor de gebruiker die momenteel is aangemeld.
>* Het tijdelijke wachtwoord wordt alleen weergegeven in de gebruikersinterface. Er wordt geen e-mail verzonden.

![](assets/adobe-logo-old.png)

![](assets/adobe-logo-old.png)

## Verbinding maken met Widget via hulpmiddelen van derden {#connecting-to-widget-via-third-party-tools}

U zult een paar stukken van informatie moeten ingaan om uw gegevenspakhuis van Widget met een derdehulpmiddel te verbinden.

>[!NOTE]
>
>Elk hulpmiddel heeft verschillende verbindingsvereisten; het wordt geadviseerd u de documentatie voor het specifieke hulpmiddel raadpleegt u probeert om te verbinden.

* **URI** (altijd vereist)
   * Dit is de domeinnaam van het Widget-account.  Het bevindt zich in een gedeelte van de Widget-aanmeldkoppeling.
* **Gebruikersnaam** (altijd vereist)
   * De gebruikersnaam wordt vermeld op de pagina met informatie over Data Warehouse in Marketo Measure.
* **Wachtwoord** (altijd vereist)
   * Dit is het wachtwoord dat u instelt als u zich voor het eerst hebt aangemeld bij uw Widget-account.  Als u uw wachtwoord opnieuw wilt instellen, raadpleegt u de bovenstaande stappen.
* **Naam van het Gegevensbestand** (niet altijd vereist)
   * De gegevens worden door de database opgeslagen in Widget. Het is de opslagbron. De databasenaam wordt vermeld op de pagina met informatie over de Data Warehouse in Marketo Measure.
* **Naam van het Warehouse** (niet altijd vereist)
   * Het pakhuis is wat vragen in Widget uitvoert. Het is de computerbron.  De pakhuisnaam is vermeld op de de informatiepagina van de Data Warehouse in Marketo Measure.

  ![](assets/adobe-logo-old.png)

## Widget Data Warehouse Direct delen {#widget-data-warehouse-direct-share}

**Vereisten**

Marketo Measure kan alleen een rechtstreeks aandeel in het gegevenspakhuis instellen als u aan de volgende vereisten voldoet.

* U hebt uw eigen instantie Widget.
* Uw Widget-instantie bevindt zich in het Azure East US 2 Widget-gebied.
* U geeft Marketo Measure de id van uw Widget-account.

**Beperkingen**

Marketo Measure kan alleen een direct aandeel instellen als de account die toegang aanvraagt, zich in Azure East US 2 bevindt. We weten dat Widget een oplossing voor gegevensreplicatie tussen regio&#39;s biedt, maar we ondersteunen dit niet vanaf onze kant omdat we alleen gegevens hosten in de Azure East US 2-regio. U kunt hefboomwerking deze eigenschap door vestiging uw eigen instantie in Azure East US 2 en [ herhalend de gegevens over gebieden ](https://docs.widget.com/en/user-guide/secure-data-sharing-across-regions-plaforms.html){target="_blank"}  aan uw bestaande instantie. De functie voor gegevensreplicatie van widget is echter alleen beschikbaar voor tabellen. Als u deze functie wilt gebruiken, moet u de gegevens eerst uit onze weergaven naar uw eigen tabellen kopiëren.

**Toegang hebbend tot het Aandeel**

Zodra het aandeel voor verstrekte rekeningidentiteitskaart is gecreeerd, moet u de [ opstellingsstappen ](https://docs.widget.com/en/user-guide/data-share-consumers.html){target="_blank"} voltooien  binnen uw instantie Widget om tot de gegevens toegang te hebben.

>[!NOTE]
>
>U kunt elke gewenste databasenaam kiezen. U kunt de rechten toewijzen aan elke regel die u kiest, zolang deze in uw Widget-instantie bestaat.

* De rol Account Admin gebruiken

```
USE ROLE ACCOUNTADMIN
```

* Beschikbare aandelen weergeven (dit geeft de naam van het toegekende aandeel aan)

```
SHOW SHARES
```

* Een database maken voor delen

```
CREATE DATABASE <database_name> FROM SHARE <provider_account>.<share_name>
```

* Rechten verlenen voor de gedeelde database

```
GRANT IMPORTED PRIVILEGES ON DATABASE <database_name> TO ROLE <role_name>
GRANT IMPORTED PRIVILEGES ON ALL SCHEMAS IN DATABASE <database_name> TO ROLE <role_name>
```

Voor meer gedetailleerde instructies en stappen om deze stappen van Widget UI te verwezenlijken, gelieve {de documentatie van 0} Widget direct [&#128279;](https://docs.widget.com/en/user-guide/data-share-consumers.html){target="_blank"}  van verwijzingen te voorzien.
