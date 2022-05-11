## Overview
## Requirements
The following minimum requirements need to be met the DHIS2 instance;
* DHIS2 version 2.35 and above
## Installation
### Metadata Package
A metadata package is a pre-configured template of DHIS2 metadata that can be installed on standalone instance or integrated into a country or organization's existing DHIS2. The process of installing a metadata package is well documented and can be found <a href="https://docs.dhis2.org/en/topics/metadata/immunization/immunization-aggregate/installation.html">here</a>
#### Fix json conflict
When importing the package you will probably have a problem about the owner of the package metadata. The package contains the id, displayName and name of the owner user.
You can get your admin user by calling this api endpoint "your_base_url/api/users?fields=id,name,displayName&pageSize=2000" and search for your user in the result.
* Replace the id of this user "M5zQapPyTZI" by the id of your admin user.
* The displayName “admin admin” by the displayName of your admin user.
* And the name "admin" by your admin user name.
#### Additional configuration
User groups:
Add your users to MRDQA package user groups.
* MRDQA Admin: Add here the user which can have access and edit permissions to the package metadata. This group allow user to push supervision planning from app to DHIS2.
* MRDQA Data access: Add here user which can submit and view the submitted data. This group allow access to the package dashboard.
Reporting period:
Change in your convenience the period type for your national MRDQA reporting form. The default period type is quaterly, edit the data set "MDQA Data collection" to modify the period type.
Organization unit assignment:
Assign the data set "MDQA Data collection" to appropriate organisation units for the supervision activities.
