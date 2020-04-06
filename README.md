# Epimodel data repository for COVID-19

This is the repository for sharing data in the Epidemics COVID-19 project.

While the data can be useful as is, the library and toolkit to use it is [epimodel](https://github.com/epidemics/epimodel), this repo is updated asynchronously to it.

All data files (mostly CSV and HDF5) are indexed by region Code (ISOalpha2 code for countries, ISO 3166-2 for country subdivisions, see the main repo readme for details).

## Common data

* `regions.csv` - Common region set used by epimodel.
* `CSSE.csv` - John hopkins data, recoded from CSSE github

### EpidemicForecasting.org countermeasure DB

* `CMS-binary.csv` - Selected binary counter-measure features
* `CMS-0to1.csv` - Selected binary or gradual 0-1 features
* `CMS-simplified.csv` - More selected features (wrong/column format now!)

## Notes: Other data sources

* `timezones.csv` - Countries (by ISO alpha-2 code) and their timezones
* `rates.csv` - Countries (by ISO alpha-2 code) and the following based on demographic data from the UN and doi:10.1101/2020.03.09.20033357 
    `Hospitalization` fraction of COVID-19 infected needing hospitalization
    `Critical` fraction of COVID-19 infected needing intensive care
    `CaseFatalityRate` fraction of COVID-19 infected that would die (IFR or infection fatality rate in the paper)
* `verity_et_al_rates.csv` - Various rates from doi:10.1101/2020.03.09.20033357
* `age_dist_un.csv` - UN Age distribution for various regions, estimated absolute numbers

### Used

* Jogn Hopkins CSSE github
* Package `pycountries`

### For reference

* Polymath [COVID-19 data wiki page](http://michaelnielsen.org/polymath1/index.php?title=COVID-19_dataset_clearinghouse)

### Unused

* http://www.geopostcodes.com/index.php?pg=resources&file=ISO_3166_2_Regions_codes#iso
* https://gist.github.com/mindplay-dk/4755200 - marked as defunct and full of errors
