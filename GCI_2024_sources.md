# Global Cybersecurity Index 2024: data provenance

Author: International Telecommunication Union (ITU).
Download host: World Bank Data360, dataset ITU_GCI.
Retrieved: 2026-09-21. Observation year: 2024 (collection 2023-2024).
Dataset: https://data360.worldbank.org/en/dataset/ITU_GCI
ITU report: https://www.itu.int/pub/D-HDB-GCI.01-2024
ITU programme: https://www.itu.int/en/ITU-D/Cybersecurity/Pages/global-cybersecurity-index.aspx

The six CSV downloads were filtered to TIME_PERIOD = 2024 and joined using
REF_AREA (ISO3 code). Country labels come from REF_AREA_LABEL. The resulting
194-country CSV preserves full downloaded numeric precision. No values were
imputed. The gci column is the downloaded overall score, not a recomputed total.
The five pillars have equal maximum contributions of 20 points; overall GCI
ranges from 0 to 100. These measure cybersecurity commitment, not cyberattack
incidence or demonstrated effectiveness.

## Version differences and checks

Use this as the ITU 2024 series distributed by World Bank Data360, rather than
an exact transcription of the original 2024 PDF. The Data360 series and original
PDF differ in some scores beyond rounding. For example, Brazil's capacity
score in the PDF is 19.09, while the downloaded series gives
19.252142076734582. The mirror's exact overall scores equal the sum of its own
five component series. Values from the two versions were not mixed. The reason
for each difference was not independently established.

ITU also reports a country-profile printing error: El Salvador's profile was
replaced by Sierra Leone's. The downloaded El Salvador values round to the
corrected ITU profile: legal 13.00, technical 0.00, organizational 15.15,
capacity 1.02, cooperation 8.13 (overall 37.29378559225543).
Correction: https://www.itu.int/en/ITU-D/Cybersecurity/Documents/GCIv5/CountryProfiles/SLV.SVG

Checks passed: 194 unique country codes, six nonmissing numeric scores per
country, all years 2024, pillar bounds 0-20, overall bounds 0-100, and overall
score equal to the five-pillar sum within 1e-8 for every country. No regional
aggregates were included. Country names follow the download's labels.

## Columns

- country: country label from Data360
- legal, technical, organizational, capacity, cooperation: pillar scores, 0-20
- gci: published overall score in this downloaded series, 0-100
- iso3: source REF_AREA country code
- year: 2024

## Original indicator downloads

- legal: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_LEGL_SCRE.csv
- technical: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_TECH_SCORE.csv
- organizational: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_ORG_SCORE.csv
- capacity: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_CDS_SCORE.csv
- cooperation: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_COOP_SCORE.csv
- gci: https://data360files.worldbank.org/data360-data/data/ITU_GCI/ITU_GCI_GCI_OVRL_SCRE.csv

Unmodified source downloads and the official PDF are retained in data_sources/gci_2024/.
