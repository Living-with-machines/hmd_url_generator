# hmd_url_generator

This repository runs a GitHub action once a week to check for new newspapers on the British Library's repository and saves the associated URLs for downloading the data for the newspapers in the [Newspaper Collection](https://bl.iro.bl.uk/collections/9a6a4cdd-2bfe-47bb-8c14-c0a5d100501f?locale=en)

The data is stored in a JSON file `HMD_title_urls.json`. The data looks like this:

```python
{"The Express": {"1850": {"url": "https://bl.iro.bl.uk/downloads/54d974ba-fcb2-4566-a5ac-b66d85954963?locale=en", "fname": "BLNewspapers_0002642_TheExpress_1850_92c556b4-ca36-4095-9050-2e89f6534bb6.zip"}, "1855": {"url": "https://bl.iro.bl.uk/downloads/aa8b9145-a7d9-4869-8f3e-07d864238ff0?locale=en", "fname": "BLNewspapers_0002642_TheExpress_1855_aad58961-131c-416c-846f-be435bf63d38.zip"}, "1862": {"url": "https://bl.iro.bl.uk/downloads/5b450972-990c-4ed5-a979-2c3fef6d0c4a?locale=en", "fname": "BLNewspapers_0002642_TheExpress_1862_19be85f5-5e76-4fd7-995f-2c24b7de36e5.zip"}, "1864": {"url": "https://bl.iro.bl.uk/downloads/9c4f2fd6-d58c-4a57-8fac-a5dd273f8ed3?locale=en", "fname": "BLNewspapers_0002642_TheExpress_1864_68176359-717d-4878-a2ac-1228c0fb83f8.zip"}....
```

This allows you to filter the newspapers by title, year or some combination of these before downloading the material. 
