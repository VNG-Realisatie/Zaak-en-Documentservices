---
layout: page-with-side-nav
title: Compliancy Zaak- en Documentservices
---
# Compliancy Zaak- en Documentservices

## Inleiding

De standaard Zaak- en Documentservices is op 5 juni 2013 formeel vastgesteld door de StUF Regiegroep. Daarmee heeft de standaard de status ‘In gebruik’ en wordt gemeenten aanbevolen om deze standaard te gebruiken.

Voor een juiste toepassing van de standaard Zaak- en Documentservices worden door KING compliancy instrumenten ontwikkeld met als doel interoperabiliteitsproblemen tussen applicaties bij gemeenten preventief te verminderen. In de paragraaf 2.1 ”Wanneer is een softwareproduct compliant” is aangegeven wanneer een softwareproduct compliant is aan de standaard Zaak- en Documentservices.

KING adviseert gemeenten bij aanschaf van software die moet voldoen aan deze standaard gebruik te maken van de [Handreiking Levering en Acceptatievoorwaarden ICT](./documenten/130131_Leverings_en_acceptatievoorwaarden_versie_2_Definitief.pdf). Daarin zijn voorwaarden opgenomen over het gebruik van compliancy instrumenten.

Op 1 oktober 2013 heeft KING de technische professionals van leveranciers tekst en uitleg gegeven over het deze testset en het gebruik van het StUF Testplatform. Onderliggend document maakt deel uit van de compliancy instrumenten van KING.

## Doel van document

Doel van dit document is het definiëren van een standaard testset voor het testen van koppelingen die gebaseerd zijn op de Zaak- en Documentservices . Deze testset beschrijft de tests die minimaal voorafgaand aan het in productie nemen van (aangepaste of nieuwe) software door de betreffende softwareleverancier uitgevoerd moeten worden.

De testen dienen uitgevoerd te worden conform deze beschrijving en met behulp en conform de voorwaarden van het [StUF Testplatform](http://www.stuftestplatform.nl/). Voor gebruik van deze testset is een abonnement nodig op het StUF Testplatform nodig. Organisaties dienen voor zover ze nog geen abonnement hebben zich aan te melden. Zie: StUF Testplatform

Indien voldaan wordt aan alle compliancy eisen uit kan de betreffende leverancier aangeven dat het geteste softwareproduct compliant is aan de standaard Zaak- en Documentservices.

## Wanneer is een softwareproduct compliant

Een softwareproduct is compliant aan de standaard Zaak- en Documentservices (*), indien aan alle onderstaande vijf eisen wordt voldaan:

| Nr  | Eis |
|---- |---- |
| 1	  | Het betreffende softwareproduct getest is conform de eisen en voorwaarden uit onderliggende document inclusief de bijlagen en |
| 2	  | De uitvoering heeft plaatsgevonden op en conform de voorwaarden van het StUF testplatform en |
| 3	  | Een foutloos testresultaat is behaald en |
| 4	  | Finale en authentieke testrapporten openbaar zijn gemaakt op het internet en |
| 5	  | In de [GEMMA softwarecatalogus](https://www.softwarecatalogus.nl/) heeft u het authentieke testrapport uit stap 4 gepubliceerd bij het betreffende softwareproduct en aangegeven (aangevinkt) dat u compliant bent. |

(*) Hoewel een foutloos testresultaat van deze testset geen absolute zekerheid geeft van 100% interoperabiliteit tussen applicaties, geeft dit wel een goede indicatie van de kwaliteit van de ondersteuning van de standaard.

## Specificatie van testset

Leveranciers van gemeentelijke software dienen koppelingen te leveren die volledig voldoen aan de standaard. Afhankelijk van de GEMMA referentiecomponent(en) die een softwareproduct invult binnen het toepassingsgebied van de standaard, stelt de standaard andere eisen. Daardoor is de testscope niet voor alle applicaties gelijk.

De specificatie Zaak- en Documentservices beschrijft vier referentiecomponenten. Dit zijn:

* Zaaksysteem (ZS);
* Documentmanagementsysteem (DMS);
* Zaak service consumer (ZSC, de applicatie die gebruik maakt van de zaakservices) applicatie ;
* Document service consumer (DSC, de applicatie die gebruik maakt van de documentservices) applicatie.

<img src="./images/Zs-dms_applicatie_architectuur.png" width="600"/>

## Consumer en provider testen

Bij elke test is middels een P of C aangegeven of het een Provider of Consumer test betreft. Bij een provider test moet de te testen applicatie een service beschikbaar stellen aan het StUF Testplatform; het StUF Testplatform zal één of meerdere berichten versturen naar de te testen applicatie. In geval van een consumer test levert het StUF Testplatform een service aan de te testen applicatie. De te testen applicatie moet in deze gevallen één of meerdere berichten versturen naar het StUF Testplatform. Afhankelijk of een test een provider of consumer test is verwacht het StUF Testplatform dus een bericht van de te testen applicatie of verstuurt het StUF Testplatform een bericht naar de te testen applicatie.

<img src="./images/Interactiepatroon.png" width="600"/>

In de volgende paragrafen wordt per referentiecomponent/rol(*) beschreven welke testen uitgevoerd moeten worden, de testscope. Indien een softwareproduct invulling geeft aan meerdere referentiecomponenten dan is de testscope voor het softwareproduct gelijk aan de gezamenlijke testscope van alle ingevulde referentiecomponenten. Bijvoorbeeld, als een softwareproduct zowel de functionaliteit levert van de referentiecomponent Zaaksysteem als van een Document Management systeem, dan dienen zowel de testen van het referentiecomponent Zaaksysteem als Document Management systeem uitgevoerd te worden.

*Een rol kan gezien worden als een groep van referentiecomponenten die dezelfde generieke functionaliteit bieden. Een voorbeeld hiervan is de Zaakservice consumer. Indien een softwareproduct de rol van Zaakservice consumer invult dan betekent dit dat in dit softwareproduct zaakgerelateerde informatie ontstaat of wordt aangepast en dat deze informatie volgens de services uit de Zaak- en Documentservices wordt ontsloten naar een Zaaksysteem. Vrijwel elk softwareproduct kan de rol van Zaakservice consumer invullen. Denk aan vergunningsystemen, handhavingssystemen, uitkeringensysteem etc.

## Testscope Zaakservice Consumer (ZsC)

Indien een softwareproduct invulling geeft aan de rol Zaakservice consumer en alle Zaakservices ondersteunt, dan moet op het StUF Testplatform de testset Zaak- en Documentservices uitgevoerd worden voor de rol van Zaak service consumers.

Tijdens de testset uitvoering mogen geen fouten geconstateerd worden door het StUF Testplatform.

De Zaak- en Document services standaard schrijft niet voor dat een Zaakservice Consumer alle Zaakservices aan moet kunnen roepen. Indien de Zaakservice consumer slechts van een aantal services gebruik maakt dan kan de testset voor Zaakservice consumers niet uitgevoerd worden. In dat geval maakt u als leverancier een ‘eigen testset’ in het StUF Testplatform. In deze testset voegt u voor elke service die uw softwareproduct ondersteunt het gelijknamige testscenario toe.

## Testscope Zaaksysteem (ZS)

Indien een softwareproduct invulling geeft aan de referentiecomponent Zaaksysteem, dan moet op het StUF Testplatform de testset Zaak- en Documentservices uitgevoerd worden voor de referentiecomponent Zaaksysteem.

Tijdens de testset uitvoering mogen geen fouten geconstateerd worden door het StUF Testplatform.

Tijdens de testuitvoering simuleert het StUF Testplatform een Zaakservice consumer en Documentservice consumer. Er worden berichten naar het softwareproduct gestuurd waarin zowel verplichte als optionele elementen voorkomen.

## Testscope Documentservice Consumer (StUF)

Indien een softwareproduct invulling geeft aan de rol Documentservice consumer en alle Documentservices ondersteunt, dan moet op het StUF Testplatform de testset Zaak- en Documentservices uitgevoerd worden voor de rol van Documentservice consumer (StUF).

Tijdens de testset uitvoering mogen geen fouten geconstateerd worden door het StUF Testplatform.

De Zaak- en Document services standaard schrijft niet voor dat een Documentservice Consumer alle Documentservices aan moet kunnen roepen. Indien de Documentservice consumer slechts van een aantal services gebruik maakt dan kan de testset voor Documentservice consumers niet uitgevoerd worden. In dat geval maakt u als leverancier een ‘eigen testset’ in het StUF Testplatform. In deze testset voegt u voor elke service die uw softwareproduct ondersteunt het gelijknamige testscenario toe.

## Testscope: Documentservice Consumer (CMIS)

De huidige versie van de testset biedt geen testdekking voor CMIS Document Consumers.

## Testscope: Documentmanagementsysteem (DMS)

Indien een softwareproduct invulling geeft aan de referentiecomponent Document Management Systeem, dan moet op het StUF Testplatform de testset Zaak- en Documentservices uitgevoerd worden voor de referentiecomponent Documentmanagement systeem.

Tijdens de testuitvoering simuleert het StUF Testplatform een Documentservice consumer en Zaaksysteem. Er worden berichten naar het softwareproduct gestuurd waarin zowel verplichte als optionele elementen voorkomen.

Naast de berichten wordt ook getest of de Zaakgerichte CMIS repository structuur correct geïmplementeerd is. Tijdens de testset uitvoering mogen geen fouten geconstateerd worden door het StUF Testplatform.

## Beschrijving testset scenario’s

De testscenario’s behorende bij deze testset zijn beschreven in spreadsheets:


In de spreadsheat is er per referentiecomponent/rol een tabblad opgenomen waar u de testscenario’s vindt die relevant zijn voor softwareproducten die deze referentiecomponent/rol invullen. Een testscenario beschrijving bestaat uit een sequence diagram (in UML) en een tabel waarin wordt toegelicht welke acties uitgevoerd moeten worden en wat daarbij het resultaat moet zijn.

<img src="./images/Zaak-_en_Documentservices_afbeelding_1.png" width="600"/>
 
Afbeelding 2: voorbeeld scenariobeschrijving

Het sequence diagram geeft aan in welke volgorde de berichten verstuurd moeten worden door het StUF Testplatform of de te testen applicatie. De rode bolletjes geven de scenariostappen weer.

<img src="./images/Zaak-_en_Documentservices_afbeelding_2.png" width="600"/>

Afbeelding 3: voorbeeld sequence diagram

## Gebruik van het StUF Testplatform

Het StUF Testplatform is een onafhankelijk en formeel toetsinginstrument voor het testen van koppelingen gebaseerd op standaarden uit de StUF familie. Het platform is vanaf eind 2011 in productie en wordt beheerd en doorontwikkeld door KING.

Primair is het StUF Testplatform voor ICT softwareleveranciers die werkzaam zijn op de gemeentelijke markt. Zij kunnen vroegtijdig tijdens de ontwikkeling van software testen of applicatie-applicatiekoppelingen voldoen aan StUF. Leveranciers worden geacht een (preventieve) test uit te voeren op het StUF Testplatform voordat een softwareproduct in productie wordt genomen.

In de [handleiding StUF Testplatform](./documenten/Gebruikershandleiding_StUF_Testplatform.pdf) wordt verder toegelicht hoe het testplatform gebruikt kan worden.