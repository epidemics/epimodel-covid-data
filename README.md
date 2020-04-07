# Epimodel data repository for COVID-19

This is the repository for sharing data in the Epidemics COVID-19 project.

While the data can be useful as is, the library and toolkit to use it is [epimodel](https://github.com/epidemics/epimodel), this repo is updated asynchronously to it.

All data files (mostly CSV and HDF5) are indexed by region Code (ISOalpha2 code for countries, ISO 3166-2 for country subdivisions, see the main repo readme for details).

**NOTE 2020-04-6:** There has been renaming of the files to be more understandable, apologies for any inconvenience.

## Common data

### Updated

* `regions.csv` - Common region set used by epimodel
* `johns-hopkins.csv` - John hopkins data, recoded from CSSE github

### Static (or seldom updated)

* `timezones.csv` - Countries (by ISO alpha-2 code) and their timezones
* `rates.csv` - Countries (by ISO alpha-2 code) and the following based on demographic data from the UN and doi:10.1101/2020.03.09.20033357 
    `Hospitalization` fraction of COVID-19 infected needing hospitalization
    `Critical` fraction of COVID-19 infected needing intensive care
    `CaseFatalityRate` fraction of COVID-19 infected that would die (IFR or infection fatality rate in the paper)
* `verity_et_al_rates.csv` - Various rates from doi:10.1101/2020.03.09.20033357
* `age_dist_un.csv` - UN Age distribution for various regions, estimated absolute numbers from https://population.un.org/wpp/
* `estimated-infectious.csv` - The historical estimations done during the testing. (Countries sorted by ISO aplha-2 code)
* `hospital-capacity.csv` - The capacity of hospital beds counted per 100k citizens with capacity of new infectionus per
  day per 1000 citizens. Year and source URL attached. (Countries sorted by aplha-2 code)
* `max_percentage_of_infected_population_for_enough_icu.csv` - The maximal percentage of the infected the infected
  population for enaugh ICU beds. 


## EpidemicForecasting.org countermeasure DB

### Direct conversion from notion.se CSVs

* `countermeasures-features.csv` - 24 selected features
* `countermeasures-model-0to1.csv` - 9 gradual featureg (pre-processed, early selection for modeling)

### Not updated

* `countermeasures-selected-binary.csv` - 16 selected binary features (not updated)

## Notes: Other data sources

### For reference

* Polymath [COVID-19 data wiki page](http://michaelnielsen.org/polymath1/index.php?title=COVID-19_dataset_clearinghouse)

### Unused

* http://www.geopostcodes.com/index.php?pg=resources&file=ISO_3166_2_Regions_codes#iso
* https://gist.github.com/mindplay-dk/4755200 - marked as defunct and full of errors
