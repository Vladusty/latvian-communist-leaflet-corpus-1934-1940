# latvian-communist-leaflet-corpus-1934-1940

Corpus of underground leaflets from Latvian communist organizations (1934–1940) compiled for Digital Humanities and historical research.

This work is licensed under a Creative Commons Attribution 4.0 International License (CC BY 4.0).

Leaflet Text File Format:

1. Dates in Square Brackets:
   [YYYY-MM-DD…] — not earlier than the specified date
   […YYYY-MM-DD] — not later than the specified date

2. Organization Codes:
   LKP_LKJS_Vidienas_org — LKP Vidiena organization and LKJS Vidiena organization (LKP Vidienas organizācija un LKJS Vidienas organizācija)
   LKP_kareivju_org — LKP Military organization (LKP kareivju organizācija)
   SP_CK — Red Aid Central Committee (Sarkanās Palīdzības Centrālā komiteja)
   SP_Riga_committee — Red Aid Riga Committee (Sarkanās Palīdzības Rīgas komiteja)
   LKJS_Riga_committee — LKJS Riga Committee (LKJS Rīgas komiteja)
   LKP_CK_Sieviesu_centrs — LKP Central Committee Women’s Center (LKP CK Sieviešu centrs)
   LKP_LKJS_Zemgales_org_Jelgavas_committee — LKP Zemgale Regional Organization Jelgava Committee and LKJS Zemgale Regional Organization Jelgava Committee (LKP Zemgales apgabala organizācijas Jelgavas komiteja un LKJS Zemgales apgabala organizācijas Jelgavas komiteja)
   LKP_LKJS_Ventspils_committee — LKP Ventspils District Committee and LKJS Ventspils District Committee (LKP Ventspils rajona komiteja un LKJS Ventspils rajona komiteja)

3. File Structure:
   id — unique identifier
   file_name — file name
   title — leaflet title in Latvian, as published in Latvijas KP CK Partijas vēstures institūts — PSKP CK Marksisma-ļeņinisma institūta filiāle, LKP, LKJS un Sarkanās Palīdzības revolucionārās lapiņas: 1920.–1940. 3. daļa (Latvijas Valsts izdevniecība, 1963)
   author — organization(s)
   date — YYYY-MM-DD if the exact date is known; YYYY-MM if only year and month are known
   print_run — number of copies printed
   typography_name — name of the printing house
   source — source reference in Chicago style

4. Text Content
   text:
   (leaflet text)
   
5. File Name Format
   Each file follows this format:
   revl-n<id_number>-<organization_code>-<date>.txt

   revl — abbreviation of Revolucionārās lapiņas, indicating the source publication
   <id_number> — three-digit serial number, e.g., 001, 004, 123
   <organization_code> — one of the organization codes listed above
   <start_date> — earliest possible date of leaflet publication (YYYY-MM-DD)
   <end_date> — latest possible date of leaflet publication (YYYY-MM-DD or YYYY-MM if only year/month known)

   Each file follow this format:
   revl-n<id_number>-<organization_code>-<date>.txt
   revl is "Revolucionārās lapiņas" for short to understand from which book it was taken.
   
   Example:
   revl-n005-LKP_CK_LKJS_CK-1934-01.txt