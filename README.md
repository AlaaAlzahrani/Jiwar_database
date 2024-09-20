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

| N   | Code  | Language        | Supported Writing Script |
|-----|-------|-----------------|--------------------------|
| 1   | af    | Afrikaans       | Latin                    |
| 2   | ar    | Arabic          | Fully diacritized Arabic |
| 3   | bg    | Bulgarian       | Cyrillic                 |
| 4   | bs    | Bosnian         | Cyrillic, Latin          |
| 5   | ca    | Catalan         | Latin                    |
| 6   | cs    | Czech           | Latin                    |
| 7   | de    | German          | Latin                    |
| 8   | el    | Greek           | Greek                    |
| 9   | en-gb | English (GB)    | Latin                    |
| 10  | en-us | English (US)    | Latin                    |
| 11  | eo    | Esperanto       | Latin                    |
| 12  | es    | Spanish         | Latin                    |
| 13  | et    | Estonian        | Latin                    |
| 14  | eu    | Basque          | Latin                    |
| 15  | fa    | Persian         | Perso-Arabic             |
| 16  | fi    | Finnish         | Latin                    |
| 17  | fr    | French          | Latin                    |
| 18  | hr    | Croatian        | Latin                    |
| 19  | hu    | Hungarian       | Latin                    |
| 20  | hy    | Armenian        | Armenian                 |
| 21  | id    | Indonesian      | Latin                    |
| 22  | it    | Italian         | Latin                    |
| 23  | kk    | Kazakh          | Cyrillic                 |
| 24  | ko    | Korean          | Hangul                   |
| 25  | lt    | Lithuanian      | Latin                    |
| 26  | lv    | Latvian         | Latin                    |
| 27  | mk    | Macedonian      | Cyrillic                 |
| 28  | ms    | Malay           | Latin                    |
| 29  | nl    | Dutch           | Latin                    |
| 30  | no    | Norwegian       | Latin                    |
| 31  | pl    | Polish          | Latin                    |
| 32  | pt    | Portuguese      | Latin                    |
| 33  | ro    | Romanian        | Latin                    |
| 34  | ru    | Russian         | Cyrillic                 |
| 35  | sk    | Slovak          | Latin                    |
| 36  | sq    | Albanian        | Latin                    |
| 37  | sr    | Serbian         | Cyrillic                 |
| 38  | sv    | Swedish         | Latin                    |
| 39  | tr    | Turkish         | Latin                    |
| 40  | uk    | Ukrainian       | Cyrillic                 |
| 41  | ur    | Urdu            | Perso-Arabic             |

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
