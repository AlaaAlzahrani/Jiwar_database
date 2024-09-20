# Jiwar Database

Jiwar database is an open-source neighborhood database covering 40 languages. It provides three types of neighborhood information (orthographic, phonological, phonographic) for 10k-30k words per language.

## Features

- 🗣️ Supports 40 languages
- 📁 Available in:
  - [TSV](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/tsv)
  - [CSV](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/csv)
  - [XLSX](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/xlsx)
  - [TXT](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/txt)

## How to Use

1. **Navigate**: go to the [jiwar_database](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database) directory.

2. **Obtain**: download the file for the language and format you need.

3. **Query**: we recommend using the database in Excel format as it allows for fast and robust queries.

## File Structure

Each file contains 25 columns with the following information:

| Column | Name | Description |
|--------|------|-------------|
| 1 | word | The orthographic word form |
| 2 | raw_frequency | Absolute frequency in the corpus for the target word |
| 3 | freq_per_m | Frequency per million words for the target word |
| 4 | zipf | Zipf frequency scale for the target word |
| 5 | num_letters | Number of letters in the orthographic word |
| 6 | num_phonemes | Number of phonemes in the IPA transcribed word |
| 7 | IPA | The International Phonetic Alphabet transcription of the target word|
| 8 | orth_density | Number of orthographic neighbors (words differing by one letter via substitution, addition, or deletion) |
| 9 | orth_density_nbrs | List of forms of orthographic neighbors identified in 'orth_density' |
| 10 | OLD20 | Orthographic Levenshtein Distance 20 |
| 11 | orth_nbr_zipf_m | Mean Zipf frequency of orthographic neighbors |
| 12 | orth_nbr_zipf_SD | Standard deviation of Zipf frequency of orthographic neighbors |
| 13 | orth_C | Orthographic clustering coefficient |
| 14 | phon_density | Number of phonological neighbors (words differing by one phoneme via substitution, addition, or deletion) |
| 15 | phon_density_nbrs | List of forms of phonological neighbors identified in 'phon_density' |
| 16 | PLD20 | Phonological Levenshtein Distance 20 |
| 17 | phon_nbr_zipf_m | Mean Zipf frequency of phonological neighbors |
| 18 | phon_nbr_zipf_SD | Standard deviation of Zipf frequency of phonological neighbors |
| 19 | phon_C | Phonological clustering coefficient |
| 20 | pg_density | Number of phonographic neighbors (words differing by one letter and one phoneme via substitution, addition, or deletion) |
| 21 | pg_density_nbrs | List of forms of phonographic neighbors identified in 'pg_density' |
| 22 | PGLD20 | Phonographic Levenshtein Distance 20 |
| 23 | pg_nbr_zipf_m | Mean Zipf frequency of phonographic neighbors |
| 24 | pg_nbr_zipf_SD | Standard deviation of Zipf frequency of phonographic neighbors |
| 25 | pg_C | Phonographic clustering coefficient |

## Supported Languages

Here's the modified table with the writing form information added for the specified languages:

| Code | Language | Writing Script Form |
|------|----------|--------------|
| af | Afrikaans | |
| ar | Arabic | Fully diacritized Arabic |
| bg | Bulgarian | |
| bs | Bosnian | Cyrillic and Latin alphabet |
| ca | Catalan | |
| cs | Czech | |
| de | German | |
| el | Greek | |
| en-gb | English (GB) | |
| en-us | English (US) | |
| eo | Esperanto | |
| es | Spanish | |
| et | Estonian | |
| eu | Basque | |
| fa | Persian | Perso-Arabic script |
| fi | Finnish | |
| fr | French | |
| hr | Croatian | |
| hu | Hungarian | |
| hy | Armenian | |
| id | Indonesian | |
| it | Italian | |
| kk | Kazakh | |
| ko | Korean | |
| lt | Lithuanian | |
| lv | Latvian | |
| mk | Macedonian | Cyrillic alphabet |
| ms | Malay | |
| nl | Dutch | |
| no | Norwegian | |
| pl | Polish | |
| pt | Portuguese | European Portuguese |
| ro | Romanian | |
| ru | Russian | |
| sk | Slovak | |
| sq | Albanian | |
| sr | Serbian | Cyrillic alphabet |
| sv | Swedish | |
| tr | Turkish | |
| uk | Ukrainian | |
| ur | Urdu | |

## File Naming

Files in the database are named using [ISO language codes](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) (e.g., 'ar' for Arabic, 'fr' for French).

## Language Not Listed?

If your language isn't listed, you can use the [Jiwar Calculator](https://github.com/AlaaAlzahrani/Jiwar) to generate neighborhood measures for words in 90 additional language varieties.


## Citation

If you use the Jiwar database in your research, please cite:

```bibtex
@preprint{Alzahrani:2024:jiwar,
    title = "{Jiwar: A Database and Calculator for Orthographic and Phonological Neighborhood Measures for 40 Languages}",
    author = {Alaa Alzahrani},
    year = "2024",
    note = "Preprint"
}
```
