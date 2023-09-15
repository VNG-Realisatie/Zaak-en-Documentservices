---
layout: page-with-side-nav
title: Documentatie Zaak- en Documentservices
folder_files:
  - title: 20150707 Specificatie Zaak- en Documentservices v1.1.02 (pdf)
    path: documenten/20150707_Specificatie_Zaak-_en_Documentservices_v1.1.02.pdf
    group: 110
    versie: 1.1.02
    status: Onbekend
    omschrijving: 
    datum: 20151006
  - title: BIJLAGE-mapping-cmis-properties-rgbz-attributen (zip)
    path: documenten/BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    group: 110
    versie: 
    status: Definitief
    omschrijving: 
    datum: 20161012
  - title: Standaard testset Zaak en Documentservices 1.0 (zip)
    path: documenten/Testset_Zaak_en_Documentservices_1.1.zip
    group: 110
    versie: 1.3
    status: In bewerking
    omschrijving: 
    datum: 20170714
  - title: Zaak- DocumentServices 1.1.02 (zip)
    path: documenten/Zaak_DocumentServices_1_1_02.zip
    group: 110
    versie: 1.1.02
    status: Onbekend
    omschrijving: 
    datum: 20150707
  - title: BIJLAGE-mapping-cmis-properties-rgbz-attributen (zip)
    path: documenten/BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
    datum: 20161012
  - title: Mapping ZDS 1.1 en ZDS 1.2 (zip)
    path: documenten/Mapping_zds11_zds12.zip
    group: 120
    versie: 1.0
    status: 
    omschrijving: 
    datum: 20160728
  - title: Releasenotes Zaak-Documentservices 1.2 Patch 2017 Q1 (pdf)
    path: documenten/Releasenotes_Zaak-Documentservices_1.2_Patch_2017_Q1.pdf
    group: 120
    versie: 1.2 Patch 2017 Q1
    status: 
    omschrijving: Releasenotes Zaak-Documentservices 1.2 Patch 2017 Q1
    datum: 20170503
  - title: Specificatie Zaak- Documentservices v1.2 (pdf)
    path: documenten/Specificatie_Zaak-_en_Documentservices_v1.2.pdf
    group: 120
    versie: 1.2
    status: Definitief
    omschrijving: 
    datum: 20170401
  - title: XSD Schema's Zaak- Documentservices (zip)
    path: documenten/Zaak-_Documentservices_1_2.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: Goedgekeurd door de werkgoep Zaak- Documentservices tijdens de bijeenkomst op 22-03-2017
    datum: 20170401
  - title: ZDS Verwerkingssoort T of I (zip)
    path: documenten/Zds_verwerkingssoort_T_of_I.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
    datum: 20190424
---

# Documentatie

Hieronder kunt u de documentatie voor de Zaak- en Documentservices
vinden. De XSD Schema's hieronder zijn gemaakt op patch 24 van sectormodel [StUF
ZKN](https://vng-realisatie.github.io/StUF-ZKN/).

Naar aanleiding van vragen over het gebruik van attribuut
verwerkingssoort en de vulling van de waarden T of I in de zaak-
documentservices is een overzicht gemaakt ter aanvulling op de bestaande
regels uit de StUF standaard en de koppelvlak specificatie. Dit
overzicht (zds_verwerkingssoort_T_of_I) is te vinden in de documentatie
hieronder.

## Zaak- en Documentservices 1.2

<table>
	<thead>
		<tr>
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th><th>Versiedatum</th>
		</tr>
	</thead>
	<tbody>
		{% for i in page.folder_files %}
			{% if i.group == 120 %} 
				<tr>
					<td>
					  <a href="{{ i.path | base_url }}">
						{{ i.title }}
					  </a>
					</td>
					<td>{{ i.versie }}</td>
					<td>{{ i.status }}</td>
					<td>{{ i.omschrijving }}</td>
					<td>{{ i.datum }}</td>
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>

## Zaak- en Documentservices 1.1

<table>
	<thead>
		<tr>
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th><th>Versiedatum</th>
		</tr>
	</thead>
	<tbody>
		{% for i in page.folder_files %}
			{% if i.group == 110 %} 
				<tr>
					<td>
					  <a href="{{ i.path | base_url }}">
						{{ i.title }}
					  </a>
					</td>
					<td>{{ i.versie }}</td>
					<td>{{ i.status }}</td>
					<td>{{ i.omschrijving }}</td>
					<td>{{ i.datum }}</td>
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>
