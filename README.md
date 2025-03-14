# Indeed Remote Tracker

This repository contains the data behind the *Indeed Hiring Lab's* Remote Tracker data product. The frequency of the data is daily and it is refreshed each month.

## Methodology

The data in this repository are the share of remote/hybrid job postings and searches on Indeed, as a percentage of total (remote AND non-remote) job postings and searches, using a seven-day trailing average. We currently provide data for Australia, Canada, Germany, France, United Kingdom, Ireland and United States.

### Postings

The job location is identified as remote before a keyword search is performed on the job posting text to identify remote/hybrid jobs. The aggregate share of job postings in a specific location that included keywords associated specifically with remote, hybrid and flexible work arrangements (e.g. "remote work", "flexible work" and "hybrid role") is then calculated. More information about the data and methodology is available in [an accompanying note](https://www.hiringlab.org/wp-content/uploads/2023/06/Hybrid-Remote-Methodology.pdf).

### Searches

The same remote/hybrid keywords are used to identify remote/hybrid job searches (i.e. job searches on the Indeed platform) based on the job search text. The aggregate share of job searches in a specific location that included remote/hybrid keywords is then calculated.

## Data schema

### Country-level

Filename:

- `remote_postings.csv`
- `remote_postings_sector.csv`
- `remote_searches.csv`

| variable   | definition                                                                          |
|------------|-------------------------------------------------------------------------------------|
| date       | Date of observation                                                                 |
| jobcountry | Two-character [ISO 3166-1 alpha-2 country code](https://www.iban.com/country-codes) |
| remote_share_xxx      | % share of remote/hybrid job postings/searches                                      |

### Sector-level

Filename: `remote-postings-sector.csv`

| variable   | definition                                                                          |
|------------|-------------------------------------------------------------------------------------|
| date       | Date of observation                                                                 |
| jobcountry | Two-character [ISO 3166-1 alpha-2 country code](https://www.iban.com/country-codes) |
| sector     | Occupational sector label                                                           |
| remote_share_xxx      | % share of remote/hybrid job postings/searches                                      |

## License

The data generated by Indeed Hiring Lab are available under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

The data and files that we have generated are freely available for public use, as long as Hiring Lab is cited as a source.

## About Hiring Lab

[Indeed Hiring Lab](https://hiringlab.org) creates innovative data insights on the global labor market that inspire new conversations about the state of work. As the economic research arm of [Indeed](https://www.indeed.com/), the world's number one job site, Hiring Lab is driven by a team of leading economists and data scientists who provide real-time thought leadership on global labor market conditions, including hiring trends, salary information, popular skills, and employer benefits. Hiring Lab analyzes millions of data points across time collected from Indeed's proprietary job postings, resumes, and job seeker behaviors to reveal emerging trends in the United States and across the world.

The unique insights generated by Hiring Lab inform talent management, employment, and labor policy decisions for businesses, researchers, academics, and job seekers alike. Hiring Lab partners with a range of policy-making organizations and NGOs including the International Monetary Fund, the European Central Bank, and the Bank of Canada to produce timely, incisive research. Hiring Lab data is also regularly cited in prominent business publications such as The Wall Street Journal, CNN, Reuters, The Globe and Mail, Der Spiegel, and The Financial Times. Hiring Lab economists regularly speak about labor market trends at leading industry, policy, and academic conferences.

Indeed has websites in over 60 markets and 28 languages. Our economists have a deep knowledge of the factors that affect global markets and are based across the world in the United States, Canada, the United Kingdom, Ireland, Germany, France, Japan, and Australia.

If you are interested in data about other markets, please contact us at <hiringlabinfo@indeed.com>.
