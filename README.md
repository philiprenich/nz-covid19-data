# New Zealand Covid-19 Case Data

The New Zealand Ministry for Health is providing daily updates of [current Covid-19 case details on their website](https://www.health.govt.nz/our-work/diseases-and-conditions/covid-19-novel-coronavirus/covid-19-current-situation/covid-19-current-cases/covid-19-current-cases-details). These are provided as an Excel spreadsheet file and as an HTML table. For programming purposes, this isn't highly useful. This repository is the same data, converted to standard JSON format.

The MoH data is checked for changes automatically each day at 12pm, 5pm, and 11pm. However, only one conversion and updating of this repository will happen per day. Update time can be checked by looking at the JSON file latest commit date.

I'm expecting that the MoH will eventually provide their database to the public in a more direct manner than the spreadsheets. Until then, I will keep this updated.

The original data comes from the Ministry of Health, whose data is copyright under Creative Commons Attribution 4.0 International Licence. These files are copyright the same.

## Changelog

### 31 March 2020

The "confirmed" and "probable" keys are now always lowercase, regardless of what case the original spreadsheet used.

### 23 March 2020

The Ministry of Health changed their file format to be a spreadsheet with both Confirmed and Probable cases as two sheets within the same file. To match that and make things simpler, the data here is now in a single file with two keys: `confirmed` and `probable`. The filename has also changed so it is descriptive outside of this repo's context.

## Contributing

If you see any issues with the data compared with the official data, or anything is out of date, please [raise an issue](https://github.com/philiprenich/nz-covid19-data/issues) or reach out to [me on Twitter](https://twitter.com/philiprenich).

## Credits

New Zealand's [Ministry of Health](https://www.health.govt.nz).

Inspired by the New York Time's [repository](https://github.com/nytimes/covid-19-data) for US Covid-19 data.

