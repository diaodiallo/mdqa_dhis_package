## Overview
This DHIS2 package is designed to work with an <a href="https://github.com/diaodiallo/mrdqa_distributions">android mobile application</a>, this package dataset is populated by this application after countries supervision activities. 
## Requirements
The following minimum requirements need to be met by the DHIS2 instance;
* DHIS2 version 2.35 and above
## Installation
### Metadata Package
A metadata package is a pre-configured template of DHIS2 metadata that can be installed on standalone instance or integrated into a country or organization's existing DHIS2. The process of installing a metadata package is well documented and can be found <a href="https://docs.dhis2.org/en/topics/metadata/immunization/immunization-aggregate/installation.html">here</a>
### Additional configurations
#### User groups:
Add your users to MRDQA package user groups.
* MRDQA Admin: Add here the user which can have access and edit permissions to the package metadata. This group allow user to push supervision planning from app to DHIS2.
* MRDQA Data access: Add here user which can submit and view the submitted data. This group allow access to the package dashboard.
#### Reporting period:
Change in your convenience the period type for your national MRDQA reporting form. The default period type is quarterly, edit the data set "MDQA Data collection" to modify the period type.
#### Organization unit assignment:
Assign the data set "MDQA Data collection" to appropriate organisation units for the supervision activities.
#### Data analysis
This package have six preconfigured dashboards you can however update or add dashboards/charts at your convenience.
