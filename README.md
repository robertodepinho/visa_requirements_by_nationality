# Visa Requirements Data

This repository contains a CSV file with visa requirements data for citizens from various countries traveling to different destinations. The data is sourced from Wikipedia and provides details on the type of visa required, allowed stay, and other relevant information. It is sourced from

> Wikipedia contributors. (2024). Category: Visa requirements by nationality. Retrieved Date: see last_update field in file, from https://en.wikipedia.org/wiki/Category:Visa_requirements_by_nationality

The reporsitory includes data refering to countries, territories and areas that issue passports, including disputed areas. The use of the term `country` is done only in the sake of simplicity and style and does not mean those referred to are all internationally recognized states. 

## Table of Contents
- [File Description](#file-description)
- [Data Fields](#data-fields)
- [Usage](#usage)
  - [Python Example](#python-example)
  - [R Example](#r-example)
- [Source](#source)
- [License](#license)

## File Description

The primary file in this repository is `mobility_data.csv`. It contains detailed information about the visa requirements for citizens from various countries traveling to different destinations.

## Data Fields

The CSV file contains the following columns:

- **iso3c_pass**: ISO 3166-1 alpha-3 code of the passport issuing country.
- **iso_name_pass**: Name of the passport issuing country.
- **iso3c_dest**: ISO 3166-1 alpha-3 code of the destination country.
- **iso_name_dest**: Name of the destination country.
- **country_dest**: Common name of the destination country.
- **visa_type**: Type of visa requirements (e.g., visa_required, evisa). Requirements are classified according to the types adopted by the [Global Passport Index](https://www.globalcitizensolutions.com/passport-index/).
- **visa_requirement**: Description of the visa requirement from the source Wikipedia pages.
- **allowed_stay**: Allowed duration of stay in the destination country (if specified).
- **notes**: Additional notes or special conditions regarding the visa requirement from the source Wikipedia pages.
- **pageid**: Wikipedia page ID from which the data was sourced.
- **wiki_page_title**: Title of the Wikipedia page.
- **wiki_page_url**: URL of the Wikipedia page.
- **wiki_page_revision_date**: Date of the last revision of the Wikipedia page.
- **last_update**: Date when the data was last retrieved and updated.
- **flag_missing**: Boolean flag indicating whether the data is missing or not.

## Usage

To use this data, you can load the CSV file into your preferred data analysis tool or programming language.

### Python Example

Here is an example using Python and Pandas:

```python
import pandas as pd

# Load the CSV file
df = pd.read_csv('mobility_data.csv')

# Display the first few rows of the dataframe
print(df.head())
```

### R Example

Here is an example using R:

```R
# Load necessary library
library(readr)

# Load the CSV file
df <- read_csv('mobility_data.csv')

# Display the first few rows of the dataframe
head(df)
```

## Source

The data is sourced from the Wikipedia pages under the visa requirements by nationality category: [Category:Visa requirements by nationality](https://en.wikipedia.org/wiki/Category:Visa_requirements_by_nationality).

## License

This project is licensed under a Attribution-ShareAlike 4.0 International License. See the [LICENSE](LICENSE.txt) file for more details.
