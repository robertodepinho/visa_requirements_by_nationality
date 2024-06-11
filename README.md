# Visa Requirements Data

This repository contains a CSV file with visa requirements data for citizens from various countries traveling to different destinations. The data is sourced from Wikipedia and provides details on the type of visa required, allowed stay, and other relevant information.

## Table of Contents
- [File Description](#file-description)
- [Data Fields](#data-fields)
- [Usage](#usage)
  - [Python Example](#python-example)
  - [R Example](#r-example)
- [Source](#source)
- [License](#license)

## File Description

The primary file in this repository is `visa_requirements.csv`. It contains detailed information about the visa requirements for citizens from various countries traveling to different destinations.

## Data Fields

The CSV file contains the following columns:

- **iso3c_pass**: ISO 3166-1 alpha-3 code of the passport issuing country.
- **iso_name_pass**: Name of the passport issuing country.
- **iso3c_dest**: ISO 3166-1 alpha-3 code of the destination country.
- **iso_name_dest**: Name of the destination country.
- **country_dest**: Common name of the destination country.
- **visa_type**: Type of visa required (e.g., visa_required, evisa).
- **visa_requirement**: Description of the visa requirement.
- **allowed_stay**: Allowed duration of stay in the destination country (if specified).
- **notes**: Additional notes or special conditions regarding the visa requirement.
- **pageid**: Wikipedia page ID from which the data was sourced.
- **wiki_page_title**: Title of the Wikipedia page.
- **wiki_page_url**: URL of the Wikipedia page.
- **wiki_page_revision_date**: Date of the last revision of the Wikipedia page.
- **last_update**: Date when the data was last updated.
- **flag_missing**: Boolean flag indicating whether the data is missing or not.

## Usage

To use this data, you can load the CSV file into your preferred data analysis tool or programming language.

### Python Example

Here is an example using Python and Pandas:

```python
import pandas as pd

# Load the CSV file
df = pd.read_csv('visa_requirements.csv')

# Display the first few rows of the dataframe
print(df.head())
```

### R Example

Here is an example using R:

```R
# Load necessary library
library(readr)

# Load the CSV file
df <- read_csv('visa_requirements.csv')

# Display the first few rows of the dataframe
head(df)
```

## Source

The data is sourced from the Wikipedia page: [Visa requirements for Afghan citizens](https://en.wikipedia.org/wiki/Visa_requirements_for_Afghan_citizens).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
