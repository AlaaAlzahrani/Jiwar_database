# Jiwar Database

## Overview

Jiwar database is an open-source neighborhood database covering 40 languages. It provides three types of neighborhood information (orthographic, phonological, phonographic) for words.

## Features

- 🗣️ Supports 40 languages
- 📁 Available in:
  - [TSV](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/tsv)
  - [CSV](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/csv)
  - [XLSX](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/xlsx)
  - [TXT](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database/txt)

## How to Use 

1. Navigate to the [jiwar_database](https://github.com/AlaaAlzahrani/Jiwar_database/tree/master/jiwar_database) directory
   
2. Download the file for the language and format you need.

3. Query: We recommend using the database in Excel format as it allows for fast and robust queries.

## File Structure

Each file contains 25 columns with the following information:

| Column | Name | Description |
|--------|------|-------------|
| 1 | word | The lexical item |
| 2 | raw_frequency | Absolute frequency in the corpus |
| 3 | freq_per_m | Frequency per million words |
| 4 | zipf | Zipf frequency scale |
| 5 | num_letters | Number of letters in the orthographic word |
| 6 | num_phonemes | Number of phonemes in the IPA transcribed word |
| 7 | IPA | International Phonetic Alphabet transcription |
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

## File Naming

Files are named using [ISO language codes](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) (e.g., 'ar' for Arabic, 'fr' for French).

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
