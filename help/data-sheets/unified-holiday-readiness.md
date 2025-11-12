---
title: Adobe DX Solutions Unified Holidation Readiness Guide
description: Dit artikel biedt een overzicht van de gereedheid voor de feestdagen voor DX Solutions.
solution: Experience Platform, Journey Optimizer, Customer Journey Analytics, Commerce, Experience Manager, Workfront, Campaign, Analytics, Target, Marketo Engage
role: Developer, Admin, Leader, User
source-git-commit: b4b75c2c32f6265ce3fbac9f3bed888e08956982
workflow-type: tm+mt
source-wordcount: '3783'
ht-degree: 0%

---

# Adobe DX Solutions Unified Holidation Readiness Guide


De Adobe DX Solutions Unified Holiday Readiness Guide helpt u zich voor te bereiden op het feestseizoen door u te richten op proactieve planning in plaats van reactieve probleemoplossing. Het biedt praktische stappen om ervoor te zorgen dat uw instanties klaar zijn, zodat potentiële problemen tot een minimum worden beperkt voordat ze zich voordoen. Het team van Adobe brengt technische deskundigheid, een brede waaier van mogelijkheden, en bewezen methodes om het juiste niveau van steun en begeleiding-zowel technisch als strategisch-zodat uw zaken goed voorbereid is te leveren.

Volg deze best practices om ervoor te zorgen dat uw Adobe Digital Experience-oplossingen veerkrachtig, veilig en klaar zijn voor piekvakantieverkeer:

* Plan voor verhoogd verkeer.
* Vermijd grote wijzigingen tijdens piekperioden; planningsupdates voor of na het feestseizoen.
* Gebruik dashboards en alarm om prestaties te controleren en knelpunten vroegtijdig te ontdekken.
* Zorg ervoor uw geoorloofde steuncontacten bijgewerkt zijn.
* [&#x200B; de steun van Adobe van het Contact &#x200B;](https://experienceleague.adobe.com/en/docs/learning-manager/using/faq/how-to-submit-support-ticket) vooraf wanneer mogelijk.

Raadpleeg de volgende secties voor aanbevelingen voor specifieke gereedheid voor feestdagen van Adobe.

* [Adobe Experience Platform](#aep)
* [Adobe Journey Optimizer](#ajo)
* [Adobe Customer Journey Analytics](#cja)
* [Adobe Commerce](#commerce)
* [Adobe Experience Manager](#aem)
* [Adobe Marketo](#marketo)
* [Adobe Workfront](#workfront)
* [Adobe Campaign](#campaign)
* [Adobe Analytics](#analytics)
* [Adobe Target](#target)

>[!NOTE]
>
>Klik op elke sectie om deze uit te vouwen.


## Handleiding voor gereedheid voor feestdagen in Adobe Experience Platform (AEP)

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Experience Platform (AEP) te zien.**

Adobe Experience Platform (AEP) speelt een cruciale rol bij het stimuleren van realtime klantervaringen. Naarmate het feestseizoen nadert, is het van essentieel belang dat uw AEP-implementatie is geoptimaliseerd voor meer verkeer, veilige gegevensverwerking en schaalbare inname.

## Voorspelde seizoensgebonden vraag

Om zich voor te bereiden op seizoensgebonden verkeerspieken raadt Adobe aan om capaciteit te plannen en streaming profielopname te controleren. Dit omvat het voorspellen van gegevensvolumes en ervoor zorgen dat uw systeem verhoogde productie kan behandelen. Zie [&#x200B; Plan voor capaciteit en seizoensgebonden verkeer &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/dataflows/ui/monitor-streaming-profile) voor verwijzing.

## Voorbereiden op schaal

Adobe biedt verschillende strategieën om ervoor te zorgen dat uw omgeving gereed is voor vakantieverkeer:

* Toegewezen capaciteit voor sandboxen verhogen.
* Identificeer hoog-productie dataflows in [&#x200B; controledashboard &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/dataflows/ui/monitor-streaming-profile) en pas throttling of het filtreren waar nodig toe.
* De partij van het gebruik voor laag-latentie gebruikt gevallen om prestaties te optimaliseren zoals die in [&#x200B; het gebruik en de capaciteiten van de Vergunning worden beschreven: Het stromen productie beste praktijken &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/landing/license/capacity#suggestions).

Deze praktijken helpen innamebetrouwbaarheid te handhaven en latentie tijdens piekperiodes te verminderen.

## Aanbevolen werkwijzen en instructies

Adobe raadt aan de volgende stappen uit te voeren en profielen te schrijven om binnen de operationele grenzen te blijven en onderbreking van de service te voorkomen:

* [&#x200B; het stromen productie beste praktijken &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/landing/license/capacity#suggestions)
* [&#x200B; Guardrails voor de Ingestie van Gegevens &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/ingestion/guardrails)
* [&#x200B; StandaardGaranties voor gegevens en segmentatie van het Profiel van de Klant in real time &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/profile/guardrails)
* [&#x200B; de Blauwdrukken van AEP: Guardrails &#x200B;](https://experienceleague.adobe.com/en/docs/blueprints-learn/architecture/architecture-overview/guardrails)

## Veiligheid en bestuur

Adobe benadrukt sterke veiligheids- en governancepraktijken, met name in de periodes met een hoog verkeersvolume, waarin de gevoeligheid van gegevens wordt vergroot.

Verwijs naar [&#x200B; Beheer, privacy, en veiligheid in Adobe Experience Platform: Veiligheid &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/overview#security) voor aanbevelingen op hoe te om klantengegevens te beschermen, privacycontroles af te dwingen, en naleving over uw implementatie van AEP te handhaven.

Door deze richtlijnen te volgen en gebruik te maken van openbare documentatie van Adobe, kunnen organisaties ervoor zorgen dat hun Adobe Experience Platform veerkrachtig, veilig en klaar is om uitzonderlijke klantervaringen te bieden gedurende het hele vakantieseizoen.

+++

## Handleiding voor gereedheid voor feestdagen in Adobe Journey Optimizer (AJO)

+++**klik om de aanbevelingen van de Adobe Journey Optimizer (AJO) holdiay gereedheid te zien.**


Om Adobe Journey Optimizer voor te bereiden op het vakantieseizoen moeten organisaties anticiperen op gebeurtenisspikes en complexiteit over het kanaal, reis- en frequentieregels configureren en zorgen voor gegevenshygiëne en besluitvormingslogica. Ze moeten ook prestaties op schaal valideren, beveiligings- en API-instructies afdwingen en inzichten na pieken toepassen om toekomstige campagnes te verfijnen.

## Voorspelende vraag

* Gebaseerd op de compressie van het vakantieseizoen en het zwaardere campagnevolume, verwacht:
   * Een piek in real-time gebeurtenissen en getriggerde reizen (autostopzetting, aanbiedingen op het laatste moment)
   * Berichtverzadigingsrisico&#39;s (hogere opt-outs, vermoeidheid)
   * Grotere complexiteit tussen kanalen (e-mail + push + SMS + in-app)
* Gebruik de cijfers van het afgelopen jaar (open/klik/opt-out tarieven, volumes van de reisingang) aan model verwachte ladingen en vastgestelde drempels voor uw overseinensystemen.
* Identificeer waarschijnlijke &quot;stille vensters&quot;of periodes van lage prestaties (bijvoorbeeld: weekends, vakantiedagen) en plan dienovereenkomstig volumes verzendt.

## Voorbereiden op schaal

* Zorg ervoor dat alle kanaalconfiguraties in AJO op de juiste wijze zijn ingesteld: e-mail, push, SMS, web, in-app. Verwijs naar [&#x200B; de configuraties van het het kanaal van de Opstelling &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/configuration/channel-surfaces).
* Configureer regels voor frequentiecapping en plafonnering om berichtvolumes te beheren. Zie het [&#x200B; het in kaart brengen van de Frequentie &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer-learn/tutorials/configuration/business-rules/configure-frequency-capping-rules) artikel.
* Vorm kanaal/de reeksen van de reisregel: Verwijs naar [&#x200B; Werk met regelreeksen &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/conflict-prioritization/capping-rules/rule-sets).
* Bereid uw gegevenshygiëne/gebeurtenisstromen in real time, en segmentatiekaders voor.
* Zorg ervoor dat u doelpubliek hebt gedefinieerd voor vakantiecampagnes, zoals:
   * hoogwaardige klanten
   * loyale segmenten
   * kar-verlaten
   * eerste kopers
* Sjablonen vooraf laden of voorbereiden voor vakantiereizen, waarbij u gebruikmaakt van besluitvormingslogica (aanbiedingen/beperkingen) zodat u zich dynamisch kunt aanpassen op basis van voorraad, tijdgevoelige aanbiedingen en kanaalvoorkeur. Zie het voorbeeld in [&#x200B; beperkingen aan een aanbiedings &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/decisioning/offer-decisioning/managing-offers-in-the-offer-library/configure-offers/add-constraints) artikel toevoegen.
* Technische gereedheid: bevestig de laadcapaciteit van de API/eindpunten, verklein/beperk de regels voor aangepaste handelingen en externe integratie. Verwijs naar [&#x200B; Grafieken en beperkingen &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/guardrails).

## Testen en valideren

* Gebruik uw experimentatieframework om belangrijke wijzigingen in variabelen te testen:
   * zendtijd
   * aanbiedingstype
   * kanaalmix
Verwijs naar [&#x200B; beste praktijken van AJO Experimentation Accelerator &#x200B;](https://experienceleague.adobe.com/en/docs/experimentation-accelerator/using/get-started/experiment-accelerator-best-practices).
* end-to-end reisvalidatie uitvoeren:
   * gebeurtenistriggers
   * segmenteringsitem
   * reispadstromen
   * personalisatielogica
   * aanbodbeperkingen
   * uitstapcriteria
* Verifieer het maximum en de collisieregels. Verwijs naar het [&#x200B; Afschilderen van de Reis &amp; arbitrage &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/conflict-prioritization/journey-capping) artikel.
* Schaalbare volumes voor piekverzendingen of piekspanningen testen: hoge triggervolumes simuleren om systeemgedrag onder belasting te valideren.
* Te leveren items valideren: e-maildomeinen/afzenders opwarmen, configuraties voor mobiele pushberichten bevestigen en fallback-kanalen controleren op SMS/in-app.

## Best practices

* Omnichannel orchestratie gebruiken. Verwijs naar het blog [&#x200B; Essentiële omnichannel klantenreizen voor overeenkomst en de groei &#x200B;](https://business.adobe.com/blog/essential-customer-journeys-for-omnichannel-engagement) artikel dat een vakantiejaarvoorbeeld met AJO toont.
* Prioriteit geven aan real-time triggers, indien van toepassing. Bijvoorbeeld: winkelwagentjes verlaten, verlaten bladeren, en voorraadalarm, aangezien de vakantiekopers reactiever zijn.
* Segmentatie en personalisatie van de hefboomwerking: doel high-intent segmenten, maak aanbiedingen op basis van eerder aankoopgedrag, en voorkeur.
* Minimale vermoeidheid bij berichten: Drijf uiteinden en rustige uren om overmatig opdrijven te voorkomen. Verwijs naar [&#x200B; de Ervaring van de Klant met het Kappen van de Frequentie van de Dagelijkse in AJO &#x200B;](https://experienceleaguecommunities.adobe.com/t5/journey-optimizer-blogs/elevate-customer-experience-with-daily-frequency-capping-in-ajo/ba-p/761510) blogpost verhogen.
* Timing is belangrijk: het plan verzendt eerder in vakantievenster (gegeven samengeperst seizoen) en richt kanalen aan tijdzones en lokaal publieksgedrag.
* Bied dynamische/beperkte tijdaanbiedingen aan om urgentie te creëren, maar coördineer over kanalen om dubbel en conflict te vermijden.
* Gebruik suppressielogica: onderdruk publiek dat zojuist heeft aangeschaft of pas postaankoopreizen toe om overbodige berichten te voorkomen.

## Veiligheid en bestuur

* Verzeker toegangsbeheer en de toestemmingen worden gevormd zodat slechts de vereiste gebruikers reizen kunnen opstellen of bedrijfsregels wijzigen.
* Controle en afdwingen API vraag/verbinding het afsnijden: Bijvoorbeeld, zie [&#x200B; Afschilderen API | Adobe Journey Optimizer &#x200B;](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/connect-systems/external-systems/capping) -artikel.
* Gebruik schone gegevens van de eerste partij en zorg voor juiste identiteitsstitching zodat het overseinen klant-centric niet dubbel/verkeerd gericht is.
* Zorg ervoor dat de leveringsdomeinen worden opgewarmd, dat er anti-spammaatregelen zijn getroffen, vooral voor vakantie met grote volumes.
* Herzie regelmatig auditlogboeken en veranderingen van de reis tijdens het piekseizoen om misstanden of foute reizen vroegtijdig op te sporen.

## Na de piek leren

* Na piekbelastingen, een overzicht van de aantallen van de reisingang, suppressietellingen, opt-out tarieven, leveringsmaatstaven, en kanaalprestaties voeren.
* Reinig onderdrukte segmenten en onderbreek of trek trajecten die zijn gemaakt voor een vakantievenster om overdraagvermoeidheid te voorkomen.
* Gebruik inzichten van prestaties in real time om de planning van volgend jaar te verfijnen (bijvoorbeeld: verzend tijdaanpassingen, kanaalmix en berichtvolume).

Door de seizoensgebonden vraag proactief te voorspellen, kanalen en regels te configureren, de reisprestaties te valideren en beveiliging en bestuur te handhaven, kunnen organisaties ervoor zorgen dat Adobe Journey Optimizer gedurende dit vakantieseizoen en daarna naadloze, gepersonaliseerde en veerkrachtige klantervaringen biedt.

+++

## Handleiding voor gereedheid voor feestdagen in Customer Journey Analytics (CJA)

+++**klik om de aanbevelingen van de de vakantiebereidheid van Customer Journey Analytics (CJA) te zien.**

Customer Journey Analytics maakt gebruik van de 5 Ps om gereed te zijn voor vakantie/piekseizoen.

### Voorbereiden op schaal

* Controleer CJA-verbindingen en gegevensweergaven en bepaal welke verbindingen en gegevensweergaven uitgebreide controle en provisioning vereisen.
* Bevestig levering voldoende voor vakantieschaal; vergroot kritieke Verbindingen en de Kijken van Gegevens zoals nodig. Zie [&#x200B; Verbindingen beheren &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-connections/manage-connections) voor meer informatie.

### Monitorprestaties

* Het RAM van de hefboomwerking ([[!UICONTROL Reporting Activity Manager] overzicht &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/reporting-activity-manager/reporting-activity-overview)) om actieve en een rij gevormde rapporteringsverzoeken in echt te controleren - tijd, bij-capaciteitsverbindingen, en vlekknelpunten te identificeren.
* Kijk voor verhoogde latentie tijdens pieklading gebruikend de [&#x200B; Gids van Fouten en van het Oplossen van problemen &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/error-messages) en [&#x200B; Bekende Beperkingen &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/aw-limitations) artikelen.
* Beheerders de mogelijkheid bieden om aanvragen die al lang lopen of geblokkeerd zijn, op voorhand te schorsen of te annuleren via RAM. Verwijs naar [&#x200B; annuleert het melden verzoeken in CJA &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/reporting-activity-manager/reporting-activity-cancel-requests) artikel.

### Best practices

* Plan de export/rapporten tijdens periodes met weinig verkeer om de belasting te verlichten en latentie te minimaliseren. Verwijs naar het [&#x200B; Geplande rapporten &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-components/scheduled-projects-manager) artikel.
* Spreid uit Verzoeken: Plan rapporten met verschillende intervallen door de dag.
* Verminder deelvensters, vereenvoudig segmenten, verkort datumbereiken en vermijd overbodige gelijktijdige taken. Zie [&#x200B; Optimizing CJA Workspace Performance &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/optimizing-performance) artikel voor details.

### Problemen oplossen

* Wanneer het oplossen van problemenwerkruimtefouten, verwijs naar foutenmeldingen voor de oorzaak en geadviseerde acties; gebruik RAM ([!UICONTROL Reporting Activity Manager]) om knelpunten te ontruimen en gelijktijdig effectief te beheren. Zie [&#x200B; CJA Workspace de Behandeling van de Fout &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/error-messages) voor meer details.
* RAM van het gebruik ([[!UICONTROL Reporting Activity Manager] in CJA &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-platform/using/reporting-activity-manager/reporting-activity-overview)) om problematische gebruikers, vragen, of projecten te identificeren; voorrang te geven aan en te beëindigen/te annuleren zoals nodig.

### Na de piek leren

* Na de vakantie/piekperiode, herzie prestaties &amp; inherente logboeken om het effect van de geleverde beste praktijken te evalueren.
* De langzame vragen van het overzicht en gebruikerstaken om patronen/tendensen te identificeren die voor het volgende seizoen kunnen worden geoptimaliseerd.
* Verzamel terugkoppelen van gebruikers en belanghebbenden—werk uw eigen runbooks en gereedheidsplannen bij met behulp van nieuw verworven inzichten.
* Feedback geven aan de Adobe-teams via uw accountteam.

+++

## Adobe Commerce-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Commerce te zien.**

Voor een succesvol piekseizoen voor uw organisatie is het van essentieel belang dat u uw Adobe Commerce digitale winkel voorbereidt op hoog verkeer.

## Voorspelende vraag

* Tijdens de piekverkoopperiode op vakantie (medio november tot medio januari) beveelt Adobe aan dat alle Adobe Commerce-handelaren die op onze cloudinfrastructuur worden gehost, proactief plannen voor een toename van het aantal bezoekers door aanvragen voor een vakantieopruimcapaciteit in te dienen. Zie {de Verzoeken van de Capaciteit van de Vakantiedruk van 0} voor Adobe Commerce op onze wolkeninfrastructuur [&#x200B; voor details.](https://experienceleague.adobe.com/en/docs/commerce-knowledge-base/kb/announcements/commerce-announcements/holiday-surge-capacity-requests-for-magento-commerce-cloud)

## Voorbereiden op schaal

Volg de aanbevelingen in de [&#x200B; Planning en het Draaien: Een strategische benadering van het piekseizoen 2025 &#x200B;](https://experienceleague.adobe.com/en/perspectives/planning-and-pivoting-a-strategic-approach-to-peak-season-2025) gids, die actionable strategieën gebruikend Adobe Commerce (en facultatieve hulpmiddelen van Adobe Experience Cloud) verstrekt om u te helpen plannen, draaien, en uitstekende klantenervaringen tijdens de drukste tijd van jaar leveren.

## Best practices

* Volg de gids van Adobe [&#x200B; hoe te om uw infrastructuur voor hoog verkeer voor te bereiden — 5 Ps van piekseizoenprestaties &#x200B;](https://business.adobe.com/blog/how-to/the-5-ps-of-peak-season-performance-a-guide-to-preparing-your-infrastructure-for-high-traffic).
* Controle uit [&#x200B; technische uiteinden voor de vakantiebereidheid van Commerce &#x200B;](https://experienceleague.adobe.com/en/docs/commerce-knowledge-base/kb/how-to/tech-tips-for-commerce-holiday-readiness) voor uiteinden op hoe te om uw infrastructuur voor hoog verkeer voor te bereiden, onderbreking te verhinderen, en prestaties in de vakantieperiode te optimaliseren.

+++

## Handleiding voor gereedheid voor Adobe Experience Manager (AEM) Cloud Services

+++**klik om de de gereedheidsaanbevelingen van de Diensten van de Wolk van Adobe Experience Manager (AEM) te zien.**

Het vakantieseizoen nadert snel, en voor veel Adobe-klanten betekent dit het begin van piekverkoopperiodes. In onze inzet voor uw succes willen wij ervoor zorgen dat u volledig voorbereid bent op de komende toename van het verkeer.

## Adobe Experience Manager (AEM) Cloud Services

Als uw organisatie de drukste momenten tijdens de vakantie ervaart, kunt u overwegen hoe te om uw plaats van Adobe Experience Manager te optimaliseren om piekverkeer aan te passen. Gelukkig beschikt uw site met Adobe Experience Manager Cloud Services al over de mogelijkheid om automatisch te schalen, zodat uw bezoekers probleemloos kunnen genieten, ongeacht of er plotselinge wijzigingen in het verkeer optreden.

## Voorbereiden op schaal

* Raadpleeg de volgende koppelingen voor gedetailleerde informatie en richtlijnen over de voorbereiding op het grote verkeer met Adobe Experience Manager Cloud Services:

   * [&#x200B; CDN in AEM as a Cloud Service &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/content-delivery/cdn)
   * [&#x200B; AEM as a Cloud Service caching &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-learn/cloud-service/caching/overview)

* Als u een Ultimate Success-klant bent en onlangs gegevens over volumeprognoses hebt gedeeld met uw Adobe-accountteam, hoeft u ons deze niet opnieuw door te sturen, aangezien we al een mening hebben.

Wij zijn hier om u in elke stap van uw reis te steunen. Voor het geval u om het even welke vragen of zorgen hebt, voel vrij om [&#x200B; een steunkaartje &#x200B;](https://experienceleague.adobe.com/en/docs/learning-manager/using/faq/how-to-submit-support-ticket) voor te leggen.

Om voor een marketing campagne in het vakantieseizoen voor te bereiden, controleer de [&#x200B; Gids van de Gebruiker AEMaaCS: Inleiding - de documentatie van de de campagneparameters van de Marketing &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/content-delivery/caching#marketing-parameters).

## Veiligheid en bestuur

Voor informatie over de veiligheid/bescherming van het de websiteverkeer van AEM, zie het [&#x200B; Overzicht - het beschermen van de websites van AEM &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-learn/cloud-service/security/traffic-filter-and-waf-rules/overview) artikel in de Zelfstudies van AEM as a Cloud Service.

## Planning voor onderhoud van vakanties

Adobe heeft geplande perioden voor het uitsluiten van onderhoud om een ononderbroken service tijdens kritieke vakantiedagen te garanderen:

* **geen automatische updates** zullen tussen voorkomen:
   * 24 november 2025 - 2 december 2025
   * 15 december 2025 - 2 januari 2026

Dit zorgt voor stabiliteit tijdens hoge-verkeersperiodes. Voor volledige versieschema&#39;s en onderhoudsvensters, verwijs naar de [&#x200B; versie roadmap van AEM &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-release-information/aem-release-updates/update-releases-roadmap).


## Adobe Experience Manager (AEM) met Adobe Managed Services (AMS)

AEM-klanten die Adobe Managed Services gebruiken, kunnen proactief met hun CSE&#39;s samenwerken om te plannen wat de dekkingsbehoeften van de feestdagen zijn.

++++

## Adobe Marketo-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Marketo te zien.**

Om succesvolle vakantiecampagnes met Adobe Marketo te verzekeren, zouden de teams e-mailauthentificatiemontages moeten verifiëren, hun gegevensbestand schoon en beveiligen, campagnecogica en planning optimaliseren, grondig het teruggeven en de leveringsbaarheid van e-mail testen, en steunbereidheid voor piekprestaties en betrokkenheid stroomlijnen.

## Voorbereiden op schaal

* Controleer uw SPF/DKIM-instellingen en controleer of alles nog steeds op de juiste wijze is ingesteld en functioneert. Zie de [&#x200B; Opstelling SPF en DKIM voor uw E-mailLeverbaarheid &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability) artikel voor details.
* U kunt uw Marketo-database controleren en opschonen door inactieve/ongeldige records op te ruimen. Hierdoor wordt de kans groter dat je land verstuurt in de postvakken van je meest verkochte kant. Zie de [&#x200B; Controle van de Gezondheid van het Gegevensbestand van Marketo &amp; hoe te het Schone &#x200B;](https://nation.marketo.com/t5/champion-program-blogs/marketo-database-health-check-up-amp-how-to-keep-it-clean/ba-p/323563) artikel voor details houden.
* Bevestig dat uw teamleden de juiste machtigingen hebben om taken uit te voeren en onbedoelde toegang of wijzigingen in de e-mails te voorkomen. Of u nu wijzigingen aanbrengt via de **[!UICONTROL Admin]** of via de **[!UICONTROL Admin Console]** , we hebben u hier wel op gewezen. Zie [&#x200B; het Leiden de Rollen van de Gebruiker en het artikel van Toestemmingen &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions).
* Herzie uw integratie Launchpad om correcte authentificatie te verzekeren en om het even welke potentiële fouten op te lossen alvorens zij worden gebruikt. Zie de [&#x200B; Gids van de Ontwikkelaar van Marketo: Authentificatie &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication) artikel.

## Best practices

Efficiëntie begint met precies begrijpen hoe Marketo prioriteiten stelt en campagnes verwerkt. Geef uw campagnes het geschenk van snelheid met deze optimalisatieuiteinden.

* Begrijpen hoe Marketo prioriteit geeft aan het verwerken van stappen in de campagnestroom is van cruciaal belang om te voorkomen dat het per ongeluk uitstellen van urgente e-mails of e-mails met hoge prioriteit wordt vermeden. Zie [&#x200B; hoe de Verwerking van de Campagne &#x200B;](https://nation.marketo.com/t5/knowledgebase/how-campaign-processing-works/ta-p/248264) artikel werkt.
* Houd rekening met de slimme-lijstlogica en zorgt ervoor dat uw campagnes snel en optimaal worden uitgevoerd. Zie [&#x200B; Beste praktijken voor Slimme Lijsten &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/best-practices-for-smart-lists) artikel.
* **[!UICONTROL Head Start]** of **[!UICONTROL Recipient Time Zone]** kan e-mails samenstellen voordat u de berichten verzendt, vertragingen reduceren en extra voorbereidingstijd voor kwalificerende leads bieden met logica met hoge resources. Zie het [&#x200B; Begin van het Kop voor E-mailProgramma&#39;s &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs) en [&#x200B; E-mailProgramma&#39;s van het Programma met de Ontvankelijke artikelen van de Streek van de Tijd &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone) voor details.
* Uw campagne is actief, en de leads stromen door, en dan merkt u een fout met stroomstap. Het is verleidelijk om met een snelle aanpassing te repareren, maar bewust zijn van wat gebeurt wanneer u een levende wachtstap verandert of uw stromen herordent kan u helpen veel hoofdpijnen en schoonmaak later vermijden. Zie de [&#x200B; het Uitgeven Stroom van de Campagne met Leden in Wacht Artikel van de Stappen &#x200B;](https://nation.marketo.com/t5/knowledgebase/editing-campaign-flow-with-members-in-wait-steps/ta-p/254294).

## Testen en valideren

Voordat u op **[!UICONTROL Send]** tikt, moet u ervoor zorgen dat de e-mails er precies zo uitzien en er naar wens uitzien.

* Marketo biedt meerdere manieren om de weergave van een e-mail te testen om te controleren of deze er precies zo uitziet als u hebt voorzien.
   * Gebruik de functie **[!UICONTROL Preview]** om ervoor te zorgen dat de dynamische inhoud en tokens correct worden weergegeven door een voorvertoning weer te geven door segmentatie of individuele leads. Zie [&#x200B; Voorproef een E-mail met Dynamische Inhoud &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content) artikel.
   * Verzend snel en eenvoudig een directe e-mail naar uw testrecords om te zien hoe uw e-mail er op verschillende clients/apparaten uitziet. Zie de [&#x200B; Looppas een Enige Stap van de Stroom van een Slimme artikel van de Lijst &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list).
   * Voor [!DNL Litmus] -gebruikers is het nu eenvoudiger dan ooit om uw account te integreren en rechtstreeks vanuit de e-maileditor renderingtests te starten. Zie [&#x200B; E-mail die van de Test met  [!DNL Litmus] teruggeeft &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/test-email-rendering) artikel.
* Controle uit de eigenschap van het E-mailspamrapport, die met [!DNL SpamAssassin] integreert om de inhoud van uw e-mail te herzien en een score toe te wijzen op hoe waarschijnlijk het inbox moet raken of als *spam* worden gemerkt. Zie het [&#x200B; E-mail spamrapport &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/spam-report) artikel.
* Houd [!UICONTROL Campaign Queue] in de gaten om te controleren of uw campagnes urgentie-items correct verwerken en prioriteit geven. Zie [&#x200B; Mijn lopende Campagne?](https://nation.marketo.com/t5/knowledgebase/is-my-campaign-running/ta-p/248662) artikel.

## Uw supportervaring stroomlijnen

Als er iets mis gaat, is snelheid belangrijk en Marketo Support is hier om te helpen! Neem deze gegevens op in uw ondersteuningsdossier om heen en weer te voorkomen en ons team te helpen sneller te werken aan een oplossing. Zie [&#x200B; Beste praktijken voor het Werken met de Steun van Marketo &#x200B;](https://nation.marketo.com/t5/knowledgebase/best-practices-for-working-with-marketo-support/ta-p/253491) artikel.

Met deze gids kunt u een beetje gemakkelijker rusten wetende dat u van een sterke positie begint om betrokkenheid en omzettingen tijdens dit kritieke venster te drijven. De inzet is hoog, maar je stress hoeft niet te zijn. Begin vandaag met uw voorbereidingen en maak van dit vakantieseizoen nog het meest succesvol.

+++

## Adobe Workfront-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Workfront te zien.**

Om Adobe Workfront voor te bereiden op het vakantieseizoen, zouden de teams steuncontacten moeten bijwerken, interne programma&#39;s met Adobe op één lijn brengen, belangrijke veranderingen tijdens piekvensters vermijden, en proactief automatiseringen en integraties controleren om vlotte verrichtingen te verzekeren.

## Voorbereiden op schaal

Zo zorgt u voor een soepele ondersteuning tijdens de feestdagen:

* Controleer en werk uw geoorloofde supportcontactpersonen vooraf bij.
* Bevestig dat de belangrijkste belanghebbenden beschikbaar zijn om met Steun samen te werken als de kritieke kwesties zich voordoen.
* Als het planningsproduct of de werkstroom tijdens het vakantievenster verandert, denk na plannend hen vóór midden november of na begin Januari voor beste turnaround tijden.
* Deel interne vakantieprogramma&#39;s aan uw contacten van Adobe mee om groepering te verzekeren.

## Testen en valideren

Houd informatie over Workfront-releases en test nieuwe functies in sandboxomgevingen:

* [&#x200B; voorbereidingen voor een versie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/en/docs/workfront/using/product-announcements/product-releases/release-readiness)
* [&#x200B; het Archief van de Nota&#39;s van de Versie van Workfront &#x200B;](https://experienceleague.adobe.com/en/docs/workfront/using/product-announcements/product-releases/product-releases)
* [&#x200B; Q1 2025 Overzicht van de Versie &#x200B;](https://experienceleague.adobe.com/en/docs/workfront/using/product-announcements/product-releases/release-25-q1/25-q1-release-overview)
* [&#x200B; Webinar Opname van de Versie van Workfront &#x200B;](https://experienceleague.adobe.com/en/docs/events/workfront-recordings/releases/25-1-release-webinar)

## Best practices

* Proactieve planning: identificeer om het even welke systeemgebiedsdelen of geplande automatiseringen die door interne onderbrekingsprogramma&#39;s kunnen worden beïnvloed.
* Doorlopende communicatie: houd uw interne teams en Adobe Support op de hoogte van gepland onderhoud of belangrijke gebeurtenissen.
* Gebruik dashboards: controleer zeer belangrijke integratie en automatisering om vroege tekenen van prestatieskwesties te vangen.
* Escalate Vroege: Als u de dienstdegradatie anticipeert of waarneemt, open onmiddellijk een steunkaartje — wacht niet tot het kritiek wordt.

Door vooruit te plannen, duidelijke communicatie te handhaven en problemen vroegtijdig te escaleren, kunnen organisaties verstoringen minimaliseren en ervoor zorgen dat Workfront gedurende de vakantieperiode kritieke workflows blijft ondersteunen.

+++

## Adobe Campaign-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Campaign te zien.**


Om Adobe Campaign op vakantiebereidheid voor te bereiden, zouden de teams online leveringsmontages proactief moeten bevestigen, publiekssegmentatie en berichtfrequentie optimaliseren, infrastructuurscalability verzekeren, en de campagneorchestratie van de overkoepelende kanalen testen om seizoensgebonden volume en betrokkenheidspieken effectief te behandelen.

## Experttips om uw vakantiecampagnes te laten uitkomen

Net zoals het nooit te vroeg is om je vakantieboodschappen te beginnen, is het nooit te vroeg om een welwillende vakantiemarketingcampagne te beginnen. Met Adobe Campaign kunt u campagnes ontwerpen, plannen en uitvoeren die ervoor zorgen dat alle wensen van uw organisatie op het gebied van vakantie uitkomen. Maar weet je wel wat de tips zijn voor het voeren van campagnes die het jaar uit zullen eindigen met een klap? Controleer deze video, [&#x200B; uiteinden van de Expert om uw vakantiecampagnes te maken uit &#x200B;](https://experienceleague.adobe.com/en/docs/events/experience-league-live-recordings/episodes/exl-live-episode-03), die leverbaarheid en uitvoerings beste praktijken bespreekt en u zal tonen hoe te om het allen in Adobe Campaign te doen.

## Overwegingen en voorbereidingen voor de vakantieperiode

Deze video, [&#x200B; Adobe Campaign: Readiness van de Vakantie - Overwegingen en Voorbereidingen voor de Periode van de Vakantie &#x200B;](https://helpx.adobe.com/customer-care-office-hours/campaign/campaign-holiday-readiness.html), behandelt:

* De Campagne-gemeenschap inschakelen
* Leverbaarheid - Overwegingen voor de vakantie en daarna!
* Technische aanbevelingen voor Adobe Campaign Classic (ACC) en Adobe Campaign Standard (ACS)

Om Adobe Campaign klaar te hebben voor het zomerseizoen van de vakantie, zouden de organisaties de leveringscontroles moeten voltooien, campagneconfiguraties bevestigen, en ervoor zorgen de scalable infrastructuur en de dwars-kanaalorkest zijn op zijn plaats om hoog-volume, tijdgevoelige campagnes door het vakantieseizoen op een betrouwbare manier uit te voeren.

+++

## Adobe Analytics-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Analytics te zien.**

Naarmate het vakantieseizoen nadert, moeten organisaties die Adobe Analytics gebruiken proactieve stappen ondernemen om ervoor te zorgen dat gegevens accuraat, platformprestaties en rapportagebetrouwbaarheid zijn tijdens piekverkeersperiodes. Adobe biedt verschillende bronnen en best practices om teams te helpen zich effectief voor te bereiden.

## Voorspelend verkeer

Om adequate hardwaretoewijzing en systeemontvankelijkheid te verzekeren, adviseert Adobe overbrengend **piekuurslag en dagelijkse server slaan/vraagvolumes** vooraf.

* Controle [&#x200B; de piek van het Verkeer het plannen en de tijden van het de hardwaretoewijzing &#x200B;](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/traffic-management/t-traffic-schedule-spike#hardware-allocation-lead-times), aangezien het begrip hoe snel de gegevens beschikbaar worden kritiek voor besluitvorming in real time tijdens hoog-volumeperiodes is.

* Leer welke invloed gegevensbeschikbaarheid en latentie in Adobe Analytics in [&#x200B; het overzicht van de gegevenslatentie van Adobe Analytics &#x200B;](https://experienceleague.adobe.com/en/docs/analytics/technotes/latency), met inbegrip van onverwachte verkeerspikes en hardwarekwesties, en ontdek geadviseerde strategieën om gegevensvertragingen te verminderen.

## Best practices

Voor teams die gegevensfeeds gebruiken om onbewerkte analysegegevens te exporteren, biedt Adobe richtlijnen voor het optimaliseren van voederconfiguraties en het voorkomen van gemeenschappelijke valkuilen.

* [&#x200B; Beste praktijken voor de gegevensvoer van Adobe Analytics &#x200B;](https://experienceleague.adobe.com/en/docs/analytics/export/analytics-data-feed/data-feeds-best-practices)

Adobe raadt aan om snel en betrouwbaar te rapporteren tijdens de vakantie:

* [&#x200B; Optimizing Analysis Workspace prestaties &#x200B;](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/workspace-faq/optimizing-performance)
* [&#x200B; het Oplossen van problemen en beste praktijken voor Report Builder: Aanbevelingen voor het optimaliseren van verzoeken &#x200B;](https://experienceleague.adobe.com/en/docs/analytics/analyze/legacy-report-builder/troubleshoot#section_33EF919255BF46CD97105D8ACB43573F)
* {de Gids van de Componenten van 0} Analytics: Geplande rapportenrij [&#128279;](https://experienceleague.adobe.com/en/docs/analytics/components/scheduled-reports-admin)

## Planning voor onderhoud van vakanties

Adobe dwingt typisch **de vensters van de onderhoudsuitsluiting** tijdens piekvakantieperiodes af om de ononderbroken dienst te verzekeren. Klanten dienen de release- en onderhoudsplannen van Adobe via Experience League te controleren en met hun Adobe-accountteams te coördineren voor supportplanning.

Door deze richtlijnen te volgen en gebruik te maken van openbare documentatie van Adobe, kunnen organisaties ervoor zorgen dat hun Adobe Analytics-implementatie robuust is, snel reageert en klaar voor de eisen van het vakantieseizoen.

+++

## Adobe Target-gids voor gereedheid voor feestdagen

+++**klik om de aanbevelingen van de de vakantiebereidheid van Adobe Target te zien.**

Het vakantieseizoen biedt opwindende mogelijkheden voor betrokkenheid, maar het komt ook met uitdagingen zoals een toename van het verkeer en een toename van de vraag naar personalisatiesystemen. Om u te helpen bij het bieden van naadloze ervaringen tijdens deze kritieke periode, hebben we belangrijke aanbevelingen opgesteld om ervoor te zorgen dat uw Adobe Target-implementatie gereed is.

## Voorspelende vraag

Begin door verkeerspikes van 20-50% of meer te voorzien en te bevestigen dat uw infrastructuur de lading kan behandelen. Verwacht activiteiten en gegevensvolumes in Adobe Target, Analytics en AEP om verrassingen te voorkomen.

Het is ook belangrijk om opdracht-kritieke reizen-zulke als controle, productaanbevelingen, en promotionele aanbiedingen-zo verpersoonlijkingsinspanning te identificeren zich concentreren waar zij het belangrijkst zijn.

Verwijs naar [&#x200B; Beste praktijken voor optimalisering met Adobe Target &#x200B;](https://experienceleague.adobe.com/en/docs/target-learn/tutorials/administration/strategy/target-best-practices-for-optimization).

## Voorbereiden op schaal

* Plan meer verkeer op de website en mobiele apparaten en informeer het team van de Steun van het Doel om servercapaciteit te verhogen om om het even welke geblokkeerde vraag te vermijden.
* Voor het testen van de lading/pen moet het ondersteuningsteam van het Doel vooraf op de hoogte worden gebracht.
* Voer een upgrade uit naar de nieuwste versies van de API voor `at.js`/Delivery.
* Niet-essentiële wijzigingen bevriezen; voorbereiden op fallback-ervaringen.
* Richt steun en escalatieprocessen en laat pro-actieve alarm toe.

## Testen en valideren

Valideer inhoudslevering gebruikend [&#x200B; verbindingen QA &#x200B;](https://experienceleague.adobe.com/en/docs/target/using/activities/activity-qa/activity-qa) om alles te bevestigen werkt zoals verwacht. Gebruik de schakeloptie **[!UICONTROL Match audience rules to see experiences]** om ervoor te zorgen dat het juiste publiek in aanmerking komt voor de activiteit die u test. Controleer of de **[!UICONTROL Goal Metric]** -configuratie is uitgelijnd op de **[!UICONTROL Objective]** -activiteit. En heb altijd een back-upplan klaar — voor het geval dat.

## Best practices

Houd uw implementatie binnen [&#x200B; de grenzen van Adobe Target &#x200B;](https://experienceleague.adobe.com/en/docs/target/using/troubleshoot/target-limits) en verifieer [&#x200B; naleving GDPR en CCPA &#x200B;](https://experienceleague.adobe.com/en/docs/target-dev/developer/implementation/privacy/cmp-privacy-and-general-data-protection-regulation) vooraf alvorens te lanceren. Houd minder dan 100 actieve activiteiten in stand en archiveer oudere om de zaken te stroomlijnen. Profiteer van **[!UICONTROL Auto-Allocate]**/**[!UICONTROL Auto-Target]** voor optimalisatie met AI-instellingen. Stel terugdraaiplannen en realtime monitoringdashboards in.

## Veiligheid en bestuur

Bevestig, voordat u ervaringen personaliseert, de naleving van toestemming in het kader van de GDPR en de CCPA. Sla PII&#39;s (Persoonlijk identificeerbare informatie) niet op in profielparameters en valideer API-beveiliging om klantgegevens te beschermen.

+++
