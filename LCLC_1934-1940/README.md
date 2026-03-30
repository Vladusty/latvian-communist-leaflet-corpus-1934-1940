# Latvian Communist Leaflet Corpus (1934–1940)

A digital corpus of Latvian communist underground leaflets (1934–1940) with structured metadata and text transcriptions.

## Description

The **Latvian Communist Leaflet Corpus (1934–1940)** (hereafter **LCLC**) is a structured digital corpus of underground political leaflets produced by illegal communist organizations in Latvia between **1 January 1934 and July 1940**, covering both the final months of the parliamentary period and the authoritarian regime established after the coup of Kārlis Ulmanis on 15 May 1934.

The corpus contains transcribed texts of communist propaganda leaflets as well as records for leaflets listed in the section "krājumā neievietoto lapiņu saraksts" ("list of leaflets not included in the edition") of the source edition, but whose texts are not reproduced there.

The dataset is intended for research in fields such as:
- digital humanities
- corpus linguistics
- modern history
- political history
- propaganda studies

The corpus is intended to serve as a reusable dataset for computational and historical research on political propaganda and underground movements in interwar Latvia.

---

## Corpus contents

The corpus includes:

- transcribed leaflet texts
- standardized metadata
- records for leaflet variants
- records for leaflets whose texts are not reproduced in the source edition

Leaflets originate from the period **1934–1940** and were published by various underground communist organizations.

## Corpus size

The corpus contains:

- **251 unique leaflet texts**
- **273 leaflet records with texts**, including textual variants of the same leaflet
- **458 total leaflet records**, including variants and records whose texts are not reproduced in the source edition

---

## Text statistics

For 251 unique leaflet texts, the corpus contains:

- **146929 words**
- **517445 tokens**

Average leaflet length: **585.37 words**  
Median leaflet length: **527 words**

Word counts are based on Unicode letter sequences extracted from the leaflet texts. Token counts are calculated using the tiktoken library with the cl100k_base encoding, processing only the content following the "text:" marker in each file.

---

## Leaflet variants

Some leaflets exist in multiple variants issued by different organizations or printed in different forms.

Such variants share the same numerical identifier but are distinguished by letter suffixes.

Example:  
id: 12a  
id: 12b


These records represent different versions of the same leaflet or closely related publications.

Variants may differ in:

- issuing organization
- language
- print run
- printing method
- minor textual differences

---

## File structure

Each leaflet is stored as a **plain text file (.txt)** containing metadata and the leaflet text.

Example record structure:

```
id: 1
file_name: lclc-n001-LKP_Vidienas_org_LKJS_Vidienas_org-5000-[1934-01-11…].txt
title: LKP un LKJS Vidienas organizācijas lapiņa ...
author: LKP Vidienas organizācija un LKJS Vidienas organizācija
date: [1934-01-11…]
print_run: 5000
typography_name: Spartaks
production_method: typographic
original_language: Latvian
text_language: Latvian
is_translation: False
note: ...
source: ...
text:
(leaflet text)
```

---

## Data format

All records are stored as UTF-8 encoded plain text files.

Each file contains structured metadata fields followed by the leaflet text.

Metadata fields appear at the beginning of the file, and the leaflet text begins after the field `text:`.

---

## Metadata fields

| Field | Description |
|------|-------------|
| id | leaflet identifier; variants of the same leaflet are marked with letters (e.g., 12a, 12b) |
| file_name | filename of the leaflet record |
| title | title or description of the leaflet |
| author | issuing organization |
| date | publication date (exact or approximate) |
| print_run | estimated print run |
| typography_name | printing house if known |
| production_method | typographic / rotator / shapirograph |
| original_language | language of the original leaflet |
| text_language | language of the transcription |
| is_translation | indicates whether the text is a translation prepared by the editors of the source edition |
| note | editorial note about textual differences or variants; used only when necessary |
| source | bibliographic source |
| text | transcription of leaflet text |

---

## Additional derived data

The repository also includes a manually compiled table of inferred leaflet locations:

`lclc_manual_location_table.csv`

This file is not part of the core source-based metadata.  
The location assignments were made manually by the compiler based on the issuing organizations and, in some cases, the content of the leaflets.  
They should therefore be treated as approximate research annotations rather than source metadata.

---

## Additional research annotations

The repository also includes manually compiled research annotations that are not part of the core source-based metadata.

### Manual topic annotations

`lclc_manual_topic_annotations.csv`

This file contains manual thematic annotations (or classification) assigned to individual leaflets.

The annotation system uses a hierarchical scheme:

- `manual_topic` – primary topic category (seven broad themes)
- `manual_topic_2` – secondary topic category (additional classification using the same thematic categories when applicable)
- `manual_topic_3` – more specific thematic label (when applicable)

The primary thematic categories are:
- Labour
- Foreign/War
- Youth
- Aid
- Spain
- Women
- Other

These annotations represent a **hard clustering** of leaflet texts and were created manually for research purposes.  
They should be treated as interpretative research annotations rather than source metadata.

---

## File naming convention

Leaflet filenames follow the pattern:

lclc-nID-author-print_run-date.txt

Examples:  

`lclc-n001-LKP_Vidienas_org_LKJS_Vidienas_org-5000-[1934-01-11…].txt`  
`lclc_ex-n001x-LKP_soldiers_org-unk-1934-01.txt`

Prefix meanings:

| Prefix | Meaning |
|------|---------|
| lclc | leaflet with transcribed text |
| lclc_ex | leaflet listed in the source edition whose text is not reproduced there |

Variants of the same leaflet are indicated by letters appended to the identifier (e.g., n012a, n012b).

Examples:  
`lclc-n004a-LKP_CK-3000-[…1934-01-30].txt`  
`lclc-n004b-LKP_CK-10000-1934-02.txt`

---

## Sources

All leaflet texts are taken from the publication:

Latvijas KP CK Partijas vēstures institūts — PSKP CK Marksisma-ļeņinisma institūta filiāle.  
*LKP, LKJS un Sarkanās Palīdzības revolucionārās lapiņas: 1920–1940*.  
3rd part. Rīga: Latvijas Valsts izdevniecība, 1963.

---

## Version

Current version: **1.0**

Future versions of the corpus may include additional leaflets or extended chronological coverage.

---

## License

This dataset is distributed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

You may use, share and adapt the dataset provided that proper attribution is given.

License text:  
https://creativecommons.org/licenses/by/4.0/

---

## Citation

For citation details and BibTeX, please refer to the CLARIN-LV repository entry.

---

## Author

Vladislavs Babaņins  
University of Latvia