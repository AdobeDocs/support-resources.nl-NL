---
title: Beheer bevindingen in het  [!DNL Adobe Success]  portaal
description: Deze gids verklaart hoe te om, op bevindingen in het  [!DNL Adobe Success]  Portaal toegang te hebben te interpreteren en te handelen om u te helpen productprestaties, veiligheid, en functionaliteit risico's proactively beheren.
source-git-commit: 435931272f25caa6997a16d371aafcf70cf9facd
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# De bevindingen beheren in de [!DNL Adobe Success] portal

In deze handleiding wordt uitgelegd hoe u toegang krijgt tot de bevindingen in de [!DNL Adobe Success] -portal, deze kunt interpreteren en er op kunt reageren om u te helpen productprestaties, beveiliging en functionaliteit proactief te beheren.

Op de pagina [!DNL Adobe Success] portal **[!UICONTROL Findings]** worden de problemen of risico&#39;s weergegeven die zijn gedetecteerd in uw Adobe-productexemplaar. De bevindingen omvatten prestaties, veiligheid, en functionaliteit, samen met hun status en risiconiveau. Door deze pagina te controleren kunt u problemen vroeg oplossen - voordat ze van invloed zijn op uw omgeving.

**wat zijn bevindingen?**

Bevindingen zijn waarschuwingen over ondersteuningsinzichten die worden weergegeven in de [!DNL Adobe Success] -portal. Ze wijzen op mogelijke problemen in de configuratie van uw Adobe-product, zoals vertraging van de prestaties, beveiligingsrisico&#39;s of onjuiste configuraties. Deze waarschuwingen zijn gebaseerd op telemetriegegevens die zijn verzameld via gereedschappen zoals API&#39;s, [!DNL New Relic] en [!DNL Splunk] .

**hoe worden bevindingen gecreeerd?**

De teams van Adobe bestuderen regelmatig de meest voorkomende steunkwesties en tendensen. Gebaseerd op de inzichten voegen zij nieuwe controles aan het systeem toe. Eenmaal per dag scant de [!DNL Adobe Success] -portal productgegevens om problemen op te sporen, zoals verkeerde configuraties, vastgezette taken of alles wat tot een systeemstoring kan leiden. Als een controle iets buiten het veilige bereik (zoals gedefinieerd door het product en de ondersteuningsteams van Adobe) vindt, verschijnt het als een bevinding.

**waarom belangrijke bevindingen zijn**

Het herzien van bevindingen helpt regelmatig vangstproblemen vroeg-alvorens zij uw systeem of klanten beïnvloeden. Deze pro-actieve benadering verbetert systeemstabiliteit, vermindert onderbreking, en steunt beste praktijken.

**hoe te om bevindingen** te bevestigen

Elke bevinding bevat aanbevelingen en duidelijke instructies voor het oplossen van het probleem, samen met koppelingen naar relevante documentatie, indien beschikbaar. Deel deze bevindingen met uw IT, team van de Techniek, of partner van Adobe, en werk samen om hen te richten. Als u deze problemen snel verhelpt, voorkomt u grotere problemen en blijft uw systeem probleemloos werken.


## Toegangsbevindingen

Om inzichten voor een product te bekijken:

1. Navigeer naar **[!UICONTROL Support & Insights]** .
1. Selecteer de relevante productkaart. Selecteer het tabblad **[!UICONTROL Findings]**. 

   ![ asp-steun-inzichten-bevindingen ](../../assets/asp-support-inisghts-findings.png)


1. U ziet een lijst met alle bevindingen voor het geselecteerde product.

   ![ adobe-succes-portaal-bevindingen ](../../assets/adobe-success-portal-findings.png)

1. Vanaf hier kunt u:

   ![ adobe-success-portaal-download ](../../assets/adobe-success-portal-download.png)

   * Specifieke items zoeken.
   * Exporteer de lijst met bevindingen door **[!UICONTROL Download Findings]** te selecteren. Als u een rapport voor één bevinding wilt exporteren, schakelt u het selectievakje naast de relevante bevinding onder de kolom **[!UICONTROL Finding Name]** in. Als u geen bevinding selecteert, bevat de PDF standaard een lijst met alle bevindingen.
   * Zie de details van een bevinding, inclusief een aanbevolen resolutie door een bevinding te selecteren onder **[!UICONTROL Finding Name]** . Op de pagina Details zoeken wordt de geselecteerde zoekopdracht weergegeven met extra context en een aanbeveling. Selecteer de downloadpijl om dit rapport weer te geven.


     ![ bevindingen-details ](../../assets/findings-details.png)


## Bevindingen van acties

Voer de volgende stappen uit om te controleren of elke bevinding nog steeds van toepassing is of kan worden genegeerd.

>[!NOTE] :
>
>De standaardcontroles worden uitgevoerd op uw instanties. Als de controles niet vinden dat de kwestie in uw geval aanwezig is, is er een status van **[!UICONTROL Not Detected]**.

1. Navigeer naar **[!UICONTROL Support & Insights]** .
1. Selecteer de relevante productkaart.
1. Open de tab **[!UICONTROL Findings]** . Alle bevindingen voor het geselecteerde product worden weergegeven.
1. Selecteer een item onder **[!UICONTROL Finding Name]** . Op de pagina met zoekgegevens kunt u:
   * Selecteer **[!UICONTROL Validate]** om te controleren of het probleem zich blijft voordoen (de knop **[!UICONTROL Validate]** is ontworpen als bevestiging dat het probleem is opgelost):

   ![ adobe-success-portal-validate ](../../assets/adobe-success-portal-validate.png)


   * Als het probleem zich nog steeds voordoet, wordt het volgende bericht weergegeven: *[!UICONTROL Validation complete. Finding still detected]* . Gebruik de informatie en de aanbeveling op de pagina van de Gegevens van het vinden om te onderzoeken en op te lossen.
   * Als de uitgave niet meer aanwezig is, wordt het volgende bericht weergegeven: *[!UICONTROL Validation Complete. Finding no longer detected]* . Wanneer het zoeken niet meer wordt gevonden, worden de &#39;finding grijstinten&#39; weergegeven en verandert de status in **[!UICONTROL Not Detected]** . Bevindingen met de status **[!UICONTROL Not Detected]** bevinden zich onder aan de lijst met bevindingen.
   * Als het probleem niet van toepassing of relevant voor u is, kunt u het negeren door **[!UICONTROL Dismiss]** te selecteren. Wanneer de bevinding wordt genegeerd, worden de grijstinten uitgeschakeld en verandert de status in **[!UICONTROL Dismissed]** .  Bevindingen met de status **[!UICONTROL Dismissed]** bevinden zich onder aan de lijst met bevindingen.

## De bevindingen begrijpen

* **[!UICONTROL Finding Name]** - Selecteer voor gedetailleerde inzichten en aanbevolen resolutiestappen.
* **[!UICONTROL Type]** - gecategoriseerd als *Functionaliteit*, *Prestaties*, en *Veiligheid*.
* **[!UICONTROL Risk Level]** - De ernstindicator, met visuele indicatoren.
* **[!UICONTROL Status]** - de huidige staat van het Vinden (b.v., *Gedetecteerd*, *niet Gedetecteerd*, *Ontworpen*).
* **[!UICONTROL Check Last Run]** - Tijdstempel van de laatste controle die de bevinding heeft bijgewerkt.


## Best practices

De pagina **[!UICONTROL Findings]** bevat aanbevelingen met de volgende risiconiveaus: **[!UICONTROL High]** , **[!UICONTROL Elevated]** en **[!UICONTROL Medium]** . **[!UICONTROL High]** is van essentieel belang, **[!UICONTROL Elevated]** is dringend en **[!UICONTROL Medium]** is niet-kritiek. De gezondheid en prestaties van de site behouden:

* Verbeter **[!UICONTROL High risk]** bevindingen snel, aangezien zij kritieke bedreigingen vormen.
* Los **[!UICONTROL Elevated]** -risicoproblemen snel op om escalatie te voorkomen.
* **[!UICONTROL Medium]** risicobevindingen regelmatig controleren en zo nodig handelen.




