---
layout: page-with-side-nav
title: Documenten Zaak- en Documentservices
folder_files:
  - title: 20150707_Specificatie_Zaak-_en_Documentservices_v1.1.02.pdf
    path: documenten/20150707_Specificatie_Zaak-_en_Documentservices_v1.1.02.pdf
    group: 110
    versie: 
    status: Definitief
    omschrijving: 
  - title: BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    path: documenten/BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
  - title: BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    path: documenten/BIJLAGE_B-mapping-cmis-properties-rgbz-attributen.xslx.zip
    group: 110
    versie: 
    status: Definitief
    omschrijving: 
  - title: Mapping_zds11_zds12.zip
    path: documenten/Mapping_zds11_zds12.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
  - title: Releasenotes_Zaak-Documentservices_1.2_Patch_2017_Q1.pdf
    path: documenten/Releasenotes_Zaak-Documentservices_1.2_Patch_2017_Q1.pdf
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
  - title: Releasenotes_Zaak-Documentservices_1.2_Patch_2017_Q1.pdf
    path: documenten/Releasenotes_Zaak-Documentservices_1.2_Patch_2017_Q1.pdf
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
  - title: Testset_Zaak_en_Documentservices_1.1.zip
    path: documenten/Testset_Zaak_en_Documentservices_1.1.zip
    group: 110
    versie: 
    status: Definitief
    omschrijving: 
  - title: Zaak-_Documentservices_1_2.zip
    path: documenten/Zaak-_Documentservices_1_2.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
  - title: Zaak_DocumentServices_1_1_02.zip
    path: documenten/Zaak_DocumentServices_1_1_02.zip
    group: 110
    versie: 
    status: Definitief
    omschrijving: 
  - title: Zds_verwerkingssoort_T_of_I.zip
    path: documenten/Zds_verwerkingssoort_T_of_I.zip
    group: 120
    versie: 
    status: Definitief
    omschrijving: 
---

# Documentatie

Hieronder kunt u de documentatie voor de Zaak- en Documentservices
vinden. Let op: de versie van de schema's van de Zaak- Documentservices
die bij sectormodel [StUF
ZKN](http://www.gemmaonline.nl/index.php/Sectormodellen_Zaken:_StUF-ZKN)
zijn opgenomen zijn verouderd. Voor de XSD schema's behorende bij versie
1.2 moet het bestand hier op de pagina gebruikt worden. Deze XSD
Schema's zijn gemaakt op patch 24 van sectormodel [StUF
ZKN](http://www.gemmaonline.nl/index.php/Sectormodellen_Zaken:_StUF-ZKN).

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
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th>
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
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>

## Zaak- en Documentservices 1.1

<table>
	<thead>
		<tr>
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th>
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
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>
