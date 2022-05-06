## Overview
## Requirements
The following minimum requirements need to be met the DHIS2 instance;
* DHIS2 version 2.28 and above
## Installation
### Metadata Package
A metadata package is a pre-configured template of DHIS2 metadata that can be installed on standalone instance or integrated into a country or organization's existing DHIS2. The process of installing a metadata package is well documented and can be found <a href="https://docs.dhis2.org/en/topics/metadata/immunization/immunization-aggregate/installation.html">here</a>
## Fix json issues
Replace the id M5zQapPyTZI by the id of your user, to get your user id go to API.
Replace the displayName “admin admin” by the name of your user, to get your user id go to API.
Replace the user name "admin" by your user name.
You can get these by doing this api call your_base_url/api/users?fields=id,name,displayName&pageSize=127 and looking for your name in the result.
## Change in your convenience the period type for your national MRDQA reporting. The default reporting period is quaterly.
## Package configuration
* Reportig period
The default reporting period is quaterly but you can change it to your covenience by editing the dataset "MRDQA...".
