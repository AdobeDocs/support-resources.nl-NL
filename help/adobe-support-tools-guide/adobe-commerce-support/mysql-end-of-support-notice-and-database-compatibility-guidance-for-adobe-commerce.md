---
title: MySQL einde-support en richtlijnen voor databasecompatibiliteit voor Adobe Commerce
description: Dit artikel bevat informatie over de eindtijdlijnen van MySQL en richtlijnen voor databasecompatibiliteit voor ondersteunde Adobe Commerce-versies.
solution: Commerce
source-git-commit: 2198e1882260ca17b8b99f7ed6d415791ec0d177
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# MySQL einde-support en richtlijnen voor databasecompatibiliteit voor Adobe Commerce

Dit artikel bevat belangrijke informatie over MySQL end of support (EOS) en databasecompatibiliteit voor ondersteunde Adobe Commerce-versies.
Adobe beveelt handelaren ten zeerste aan deze aankondiging te herzien en maatregelen te nemen om de stabiliteit van het platform te handhaven en te blijven voldoen aan de ondersteuningsvereisten.
Leer meer in de [&#x200B; Vereisten van de Verbetering voor MariaDB &#x200B;](https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/maintenance/mariadb-upgrade) en [&#x200B; Vereisten van het Systeem &#x200B;](https://experienceleague.adobe.com/en/docs/commerce-operations/installation-guide/system-requirements).

## MySQL 8.0 End of Support (EOS)

MySQL 8.0 bereikt einde van steun (EOS) op 30 April 2026.
Na deze datum ondersteunen of onderhouden de volgende Adobe Commerce-versies geen compatibiliteit met MySQL-versies die na MySQL 8.0 worden uitgebracht:

* Adobe Commerce 2.4.7
* Adobe Commerce 2.4.6
* Adobe Commerce 2.4.5

Adobe valideert of biedt geen ondersteuning voor nieuwere MySQL-hoofdversies in deze Adobe Commerce-releases.

## Vereiste actie voor klanten op het terrein

Adobe Commerce-installaties op locatie met de volgende versies wordt sterk aangeraden hun databaseservers te migreren naar een compatibele versie van MariaDB:

* 2.4.5.
* 2.4.6.
* 2.4.7.

MariaDB wordt volledig gesteund voor deze versies en is het geadviseerde gegevensbestandplatform dat zich verder beweegt.

* 2.4.5.
* 2.4.6.
* 2.4.7.

sterk wordt aangeraden om hun databaseservers te migreren naar een compatibele MariaDB-versie.
MariaDB wordt volledig ondersteund voor deze Adobe Commerce-versies en is het aanbevolen databaseplatform.

## MySQL-ondersteuning in Adobe Commerce 2.4.8 en 2.4.9

Adobe Commerce 2.4.8 en 2.4.9 zijn de laatste Adobe Commerce-versies die MySQL ondersteunen.

Voor deze versies:
* MySQL 8.4 is de laatste MySQL-versie die door Adobe Commerce wordt ondersteund.
* Geen MySQL-versies die na 8.4 worden uitgebracht, worden gecertificeerd of ondersteund in Adobe Commerce.

## Toekomstige richting: MariaDB als het standaarddatabaseplatform

Adobe Commerce blijft MariaDB als het standaard en aanbevolen databaseplatform ondersteunen.

Adobe raadt ten zeerste aan dat de volgende klanten hun migratie naar MariaDB beginnen te plannen om de compatibiliteit op lange termijn en de supportuitlijning te behouden:
* Alle Adobe Commerce 2.4.8- en 2.4.9-on-premisse klanten
* Klanten die eerdere ondersteunde Adobe Commerce-versies uitvoeren
