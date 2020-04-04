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

### Used

* Jogn Hopkins CSSE github
* Package `pycountries`

### For reference

* Polymath [COVID-19 data wiki page](http://michaelnielsen.org/polymath1/index.php?title=COVID-19_dataset_clearinghouse)

### Unused

* http://www.geopostcodes.com/index.php?pg=resources&file=ISO_3166_2_Regions_codes#iso
* https://gist.github.com/mindplay-dk/4755200 - marked as defunct and full of errors
