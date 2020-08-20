# PLMD\_crosswalk

| **ESS-DIVE Field** | **JSON-LD** | **DataCite 4.1** | **OSTI** | **FGDC** | **ESGF** | **CMIP6** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Title | name | title | title | CDIAC/Product\_title | title | title |
| Alternative Identifiers | alternateName | alternateIdentifiers | other\_identifying\_numbers | CDIAC/Product\_number | id | id |
| Abstract | description | description\[@type=Abstract\] | description | CDIAC/Notes |  | description \(optional\) |
| Keywords | keywords | subjects | subject | mercury/Keywords |  |  |
| Data Variables | variablesMeasured | subjects | subject | mercury/Keywords | variable | variable |
| Pulication Date | datePublished | publicationYear | publication\_date | CDIAC/Initial\_date\_of\_data\_publication |  | timestamp \(optional\) |
| Data Usage Rights | license | rightsList |  |  |  |  |
| Project | provider/name | publisher | originating\_research\_org |  | project | project |
| Funding Organizations | funder | funderReference | sponsor\_org |  |  |  |
| DOE Contracts | award |  | doe\_contract\_number |  |  |  |
| Related References | citation | relatedIdentifier | related\_resource |  |  |  |
| Contact Person First Name | editor/givenName | contributor\[@type=ContactPerson\]/givenName | contact\_name | mercury/CDIAC/CDIAC\_contact |  |  |
| Contact Person Last Name | editor/familyName | contributor\[@type=ContactPerson\]/familyName | contact\_name | mercury/CDIAC/CDIAC\_contact |  |  |
| Contact Person Organization | editor/affiliation | contributor\[@type=ContactPerson\]/affiliation | contact\_org | mercury/CDIAC/CDIAC\_contact |  |  |
| Contact Person Email | editor/email |  | contact\_email | mercury/CDIAC/CDIAC\_contact |  |  |
| Contact Person ORCID | editor/@id | contributor\[@type=ContactPerson\]nameIdentifier\[@nameIdentifierScheme=ORCID\] |  |  |  |  |
| Creator First Name | creator/givenName | creator/givenName | creators\_detail/first\_name | CDIAC/Author |  |  |
| Creator Last Name | creator/familyName | creator/familyName | creators\_detail/last\_name | CDIAC/Author |  |  |
| Creator Organization | creator/affiliation | creator/affiliation | creators\_detail/affiliation\_name | CDIAC/Author |  |  |
| Creator Email | creator/email |  | creators\_detail/private\_email | CDIAC/Author |  |  |
| Creator ORCID | creator/@id | creator/nameIdentifier\[@nameIdentifierScheme=ORCID\] | creators\_detail/orcid |  |  |  |
| Contributor First Name | contributor/givenName | contributor\[@type=Other\]/givenName | contributor/first\_name |  |  |  |
| Contributor Last Name | contributor/familyName | contributor\[@type=Other\]/familyName | contributor/last\_name |  |  |  |
| Contributor Organization | contributor/affiliation | contributor\[@type=Other\]/affiliation | contributor/affiliation\_name |  |  |  |
| Contributor Email | contributor/email |  | contributor/private\_email |  |  |  |
| Contributor ORCID | contributor/@id | contributor\[@type=Other\]nameIdentifier\[@nameIdentifierScheme=ORCID\] | contributor/orcid |  |  |  |
| Start Date | temporalCoverage | dates/date |  | timeinfo/rngdates/begdate | datetime\_start \(optional for Earth Sciences\) | datetime\_start \(optional\) |
| End Date | temporalCoverage | dates/date |  | timeinfo/rngdates/enddate | datetime\_stop\( option for Earth Sciences metadata\) | datetime\_stop \(optional\) |
| Location Description | spatialCoverage/description | geoLocation/geoLocationPlace | geolocation/place | CDIAC/Site\_info/Site\_name |  |  |

