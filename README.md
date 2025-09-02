# Latvian Communist Leaflet Corpus (1934–1940)

## About the Project

The **`latvian-communist-leaflet-corpus-1934-1940`** is a digital collection of underground agitational materials issued by various communist and pro-communist organizations in Latvia from 1934 to 1940. The project's goal is to create a structured and easily accessible body of texts for use in historical research, linguistic analysis, and Digital Humanities projects.

All texts have been transcribed from the publication: `Latvijas KP CK Partijas vēstures institūts — PSKP CK Marksisma-ļeņinisma institūta filiāle, LKP, LKJS un Sarkanās Palīdzības revolucionārās lapiņas: 1920.–1940. 3. daļa (Latvijas Valsts izdevniecība, 1963)`.

---

## Repository Structure

### Main Directories

* **`latvian_communist_leaflets_1934-1940/`**: This is the main directory for the ready-to-use corpus. It currently contains 28 files, with more to be added as the project progresses. Each file represents a single leaflet with structured metadata.
* **`for_editing/`**: A working directory for the transcription and editing process. It contains `revl-all-LKP_leaflets-1934-1940.docx`, which serves as a staging ground for texts before they are finalized and moved to the main corpus.

### File Content

Each text file in the main corpus (`latvian_communist_leaflets_1934-1940/`) follows a consistent structure:

**Metadata**
* **`id`**: The unique serial number for the leaflet.
* **`file_name`**: The full file name.
* **`title`**: The title of the leaflet in Latvian, as found in the source.
* **`author`**: The full name of the organization(s) responsible for the leaflet.
* **`date`**: The publication date.
    * Format: `YYYY-MM-DD` (if the exact date is known) or `YYYY-MM` (if only the month and year are known).
    * Approximate dates use square brackets: `[YYYY-MM-DD...]` (not earlier than the specified date) or `[...YYYY-MM-DD]` (not later than the specified date).
* **`print_run`**: The number of copies printed, as recorded in the source.
* **`typography_name`**: The name of the underground printing house, if known.
* **`source`**: The bibliographic citation for the source.

**Text Body**
* **`text:`**: The full, transcribed text of the leaflet.

### File Naming Convention

The files in the main corpus are named using a strict format: `revl-n<id_number>-<organization_code>-<date>.txt`.

* `revl` — Short for `Revolucionārās lapiņas`, indicating the source book.
* `<id_number>` — A three-digit serial number (e.g., `001`).
* `<organization_code>` — A code for the issuing organization. A complete list of codes is provided in the `for_editing/` directory.
* `<date>` — The date of publication.

**Example:** `revl-n002-LKP_kareivju_org-[1934-01-11...].txt`

---

## License

This work is licensed under a  
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

---

## Author

- **Vladislavs Babaņins**
