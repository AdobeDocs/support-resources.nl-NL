---
title: Fout bij samenvouwen van secties
description: UGP-13446 toe te vouwen gedeelten worden niet gerenderd, mogelijk vanwege ingesloten paginatabbladen
hide: true
hidefromtoc: true
source-git-commit: f2d8eb9125df5f542c1ed075348586965f4adaad
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 6%

---

# Inklapbare secties

<http://jira.corp.adobe.com/browse/UGP-13446> UGP-13446 toe te vouwen gedeelten worden niet gerenderd, mogelijk vanwege ingesloten paginatabbladen

## Voorbeelden

Eerste met paginatabbladen; tweede zonder

### Optie 2: Met paginatabbladen

+++ Handmatige hotfix-installatie voor 6.5.18.0 - 6.5.22.0

**Stap 1: De download en trekt het Hotfix Pakket** uit

- Download [ hotfix voor 6.5.18.0 - 6.5.22 ](https://www.adobe.com) van het Portaal van de Distributie van de Software van Adobe
- Lokaal extraheren

**Stap 2: Navigeer aan de Correcte Omslag van de Versie**

- Op basis van de versie Service Pack die op uw omgeving is geïnstalleerd, gaat u naar de overeenkomende map.

  Voorbeeld voor Service Pack 20 is de map:

  ```
  <extracted-hotfix>/SP20/
  ```

**Stap 3: Bepaal de plaats van de Folder van de Plaatsing**

- Ga op uw AEM Forms op de JEE-server naar:

  ```
  [AEM installation directory]/deploy
  ```

  Voorbeeld: `adobe/adobe-experience-manager-forms/deploy`



**Stap 4: Werk en vervang de dossiers van het EAR** bij

>[!BEGINTABS]

>[!TAB  JBoss ]

1. `adobe-core-jboss.ear` openen en `adminui.war` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/jboss/adminui.war
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/jboss/adminui.war`

1. Ga in de `adobe-core-jboss.ear` naar de `lib/` map en vervang `adobe-uisupport.jar` door:

   ```
   adobe-xxe-configuration-hotfix/SP[version]/adobe-uisupport.jar
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/adobe-uisupport.jar`

1. Sla het EAU op. Controleer of de wijzigingen correct zijn opgeslagen.


1. `adobe-edcserver-jboss.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/jboss/adobe-edcserver-jboss.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/jboss/adobe-edcserver-jboss.ear`

1. `adobe-forms-jboss.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/jboss/adobe-forms-jboss.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/jboss/adobe-forms-jboss.ear`



>[!TAB  WebLogic ]

1. `adobe-core-weblogic.ear` openen en `adminui.war` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/weblogic/adminui.war
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/weblogic/adminui.war`

1. In de `adobe-core-weblogic.ear` vervangt u `adobe-uisupport.jar` door:

   ```
   adobe-xxe-configuration-hotfix/SP[version]/adobe-uisupport.jar
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/adobe-uisupport.jar`

1. Sla het EAU op. Controleer of de wijzigingen correct zijn opgeslagen.


1. `adobe-edcserver-weblogic.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/weblogic/adobe-edcserver-weblogic.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/weblogic/adobe-edcserver-weblogic.ear`

1. `adobe-forms-weblogic.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/weblogic/adobe-forms-weblogic.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/weblogic/adobe-forms-weblogic.ear`

>[!TAB  WebSphere ]

1. `adobe-core-websphere.ear` openen en `adminui.war` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/websphere/adminui.war
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/websphere/adminui.war`

1. In de `adobe-core-websphere.ear` vervangt u `adobe-uisupport.jar` door:

   ```
   adobe-xxe-configuration-hotfix/SP[version]/adobe-uisupport.jar
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/adobe-uisupport.jar`

1. Sla het EAU op. Controleer of de wijzigingen correct zijn opgeslagen.


1. `adobe-edcserver-websphere.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/websphere/adobe-edcserver-websphere.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/websphere/adobe-edcserver-websphere.ear`

1. `adobe-forms-websphere.ear` vervangen door

   ```
   adobe-xxe-configuration-hotfix/SP[version]/websphere/adobe-forms-websphere.ear
   ```

   Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/websphere/adobe-forms-websphere.ear`

>[!ENDTABS]



**Stap 5: Update `adobe-rightsmanagement-<appserver>-dsc.jar` dossier met**

```
adobe-xxe-configuration-hotfix/SP[version]/<appserver>/adobe-rightsmanagement-<appserver>-dsc.jar
```

Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/jboss/adobe-rightsmanagement-jboss-dsc.jar`

**Stap 6: De extra Configuratie voor de Veiligheid van het Document op WebSphere en WebLogic**:

Als u Documentbeveiliging gebruikt (voorheen Rights Management), stelt u de volgende Java-systeemeigenschap (JVM-argument) in voordat u de AEM Forms-server start:

```
-Dcom.adobe.forms.jee.services.allowDoctypeDeclaration=true
```


**Stap 7: Voer de Manager van de Configuratie** opnieuw in

- Start de configuratiemanager om het bijgewerkte EAR opnieuw te implementeren en de hotfix toe te passen

+++

### Optie 2: Zonder paginatabbladen

+++ Handmatige hotfix-installatie voor 6.5.18.0 - 6.5.22.0

**Stap 1: De download en trekt het Hotfix Pakket** uit

- Download [ hotfix voor 6.5.18.0 - 6.5.22 ](https://www.adobe.com) van het Portaal van de Distributie van de Software van Adobe
- Lokaal extraheren

**Stap 2: Navigeer aan de Correcte Omslag van de Versie**

- Op basis van de versie Service Pack die op uw omgeving is geïnstalleerd, gaat u naar de overeenkomende map.

  Voorbeeld voor Service Pack 20 is de map:

  ```
  <extracted-hotfix>/SP20/
  ```

**Stap 3: Bepaal de plaats van de Folder van de Plaatsing**

- Ga op uw AEM Forms op de JEE-server naar:

  ```
  [AEM installation directory]/deploy
  ```

  Voorbeeld: `adobe/adobe-experience-manager-forms/deploy`



**Stap 4: Werk en vervang de dossiers van het EAR** bij

Pagina tabs verwijderd

**Stap 5: Update `adobe-rightsmanagement-<appserver>-dsc.jar` dossier met**

```
adobe-xxe-configuration-hotfix/SP[version]/<appserver>/adobe-rightsmanagement-<appserver>-dsc.jar
```

Bijvoorbeeld: `adobe-xxe-configuration-hotfix/SP20/jboss/adobe-rightsmanagement-jboss-dsc.jar`

**Stap 6: De extra Configuratie voor de Veiligheid van het Document op WebSphere en WebLogic**:

Als u Documentbeveiliging gebruikt (voorheen Rights Management), stelt u de volgende Java-systeemeigenschap (JVM-argument) in voordat u de AEM Forms-server start:

```
-Dcom.adobe.forms.jee.services.allowDoctypeDeclaration=true
```


**Stap 7: Voer de Manager van de Configuratie** opnieuw in

- Start de configuratiemanager om het bijgewerkte EAR opnieuw te implementeren en de hotfix toe te passen

+++

Fin
