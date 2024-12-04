## Overview
This DHIS2 package is designed to work with an <a href="https://github.com/diaodiallo/mrdqa_distributions">android mobile application</a>, its dataset is populated by this application after countries supervision activities. From the version 2.x of this package you need the 5.x or later version of the Android app.
## Requirements
The following minimum requirements need to be met by the DHIS2 instance;
* DHIS2 version 2.35 and above
## Installation
### Metadata Package
A metadata package is a pre-configured template of DHIS2 metadata that can be installed on standalone instance or integrated into a country or organization's existing DHIS2. The process of installing a metadata package is well documented and can be found <a href="https://docs.dhis2.org/en/topics/metadata/immunization/immunization-aggregate/installation.html">here</a>
### Additional configurations
#### JSON file preparation
After downloading the metadata package json file you need to replace the word "ADMIN_ID" with an admin user id of your DHIS2 instance or any user that has permissions to create metadata. You can get the user id by going to the user profile and copy the id from the url.
#### User groups:
Add your users to MRDQA package user groups.
* MRDQA Admin: Add here the user which can have access and edit permissions to the package metadata. This group allow user to push supervision planning from app to DHIS2.
* MRDQA Data access: Add here user which can submit and view the submitted data. This group allow access to the package dashboard.
#### Reporting period:
Change in your convenience the period type for your national MRDQA reporting form. The default period type is quarterly, edit the data set "MRDQA Data collection" to modify the period type. If you modify the default period type you need to update the period type for all the dashboard visualizations.
#### Organization unit assignment:
Assign the data set "MRDQA Data collection" to appropriate organisation units for the supervision activities.
#### Data analysis
This package has seven preconfigured dashboards you can however update or add dashboards/charts at your convenience.
