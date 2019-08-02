# Analysis:
My analysis revolves around checking what percentage of along with which websites and scripts in this dataset are tracking users location (geolocation) and language preferences as well as their country code. So, as to provide them with a customized content based on the users preferences (eg. location, language)

### Dataset used: Sample 10 percent
[sample 10 percent - 3.7GB download / 7.4GB on disk](https://public-data.telemetry.mozilla.org/bigcrawl/sample_10percent.parquet.tar.bz2)


# Inference:
## Overall:
- Out of the total of **205949** websites/locations in this dataset **46482** `(22.57%)` websites were found to be checking for preferred language of the user, usually the language of the browser UI, and their subsequent location/scripts can be found in the `language_pref_df` dataframe.

- Out of the total of **205949** websites/locations in this dataset **2216** `(1.08%)` websites were found to be checking for user's location using the geolocation api, and their subsequent location/scripts can be found in the `geolocation_df` dataframe.

## Scripts:
- Out of the total of **166862** scripts in this dataset **7700** `(4.61%)` scripts were found to be making the calls to check for preferred language of the user, usually the language of the browser UI, and their subsequent scripts can be found in the `language_pref_df.script_url` dataframe.

- Out of the total of **166862** scripts in this dataset **1359** `(0.81%)` scripts were found to be making the calls to check for user's location using the geolocation api, and their subsequent scripts can be found in the `geolocation_df.script_url` dataframe.

## Domains:
- For geolocation tracking: scripts were being executed from `400` unique domains (`geolocation_unique_domains`).
- For language & country code tracking: scripts were being executed from `2271` unique domains (`language_pref_unique_domains`).
