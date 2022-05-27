# Dataset metadata guide

This page provides guidelines and expectations for each metadata field for uploads to the ESS-DIVE repository. The JSON-LD Field Names refer to vocabulary used for submission through our [programmatic API](https://docs.ess-dive.lbl.gov/contributing-data/data-submission-guidelines/package-service-tutorial).

---

| **Title** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `name` |
| Description | Include a title between 7-20 words long which contains information such as the topic, geographic location, dates, and scale of data. If data is associated with a journal publication, the title may include the journal name. Avoid unexplained acronyms or project-specific vocabulary. If there is an existing DOI for the data, use the same title. |
| Example | Raw sapflow and soil moisture data from January 2016-April 2016 in Manaus, Brazil |
| Format | Free Text |

| **Existing DOI & Alternate Identifier** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `alternateName` |
| Description | If this dataset has been previously published elsewhere, enter the DOI or alternate identifier. Identifiers are used to locate the dataset within your project's data management system and can provide pertinent contextual information for users. Ensure the identifier correctly leads to the dataset that you are submitting.|
| Example |`http://dx.doi.org/XXXX`|
| Format | Not free text |

| **Abstract** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `description` |
| Description | The abstract should be at least 100 words in length, written in full sentences, and understandable to anyone who has not seen related manuscripts. Describe the content of the dataset, and provide all necessary scientific context, avoid unexplained acronyms or project specific terms, and include specific details that promote the reproducibility of your data. This may include source data for synthesis work, software necessary to view the related files, ecosystem type involved, or measurement types. Include a statement about the purpose for why these data were generated and the research question it is intended to answer. |
| Example |This dataset contains raw output from a data logger connected to 9 sapflow and 5 soil moisture sensors in Manaus, Brazil. The file xxx.dat contains raw data and the metadata file (BR-Ma2_E-fieldlog_20160501.xls) has information on locations where the sensors were installed and other sensor maintenance details. No data processing or QA/QC was done on the raw datasets. Processed data will be uploaded as separate datasets on ESS-DIVE. This research was performed as a part of the NGEE Tropics project, which aims to advance model predictions of tropical forest carbon cycle responses to a changing climate over the 21st Century.|
| Format | Free Text |

| **Keywords** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `keywords` |
| Description | Add a minimum of three total keywords or data variables. As you begin typing in the web form field, GCMD controlled vocabulary terms will appear in a dropdown list. Selecting from the GCMD controlled keywords where possible is encouraged but not required. You can also enter your own keywords. Ensure that keyword terms differ from words in the title to increase the findability of your dataset in searches. |
| Example |Earth Science, Land Surface, Soils|
| Format | [GCMD Keywords](https://forum.earthdata.nasa.gov/viewforum.php?f=7&&ServicesUsage=101&sid=89340eba8a64e8f66d8dcb392431831a) or Free Text |

| **Data Variables** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `variablesMeasured` |
| Description | Add variables to increase the findability of your dataset in searches. Similarly to the keywords field, selecting variable terms from GCMD controlled vocabulary where possible is encouraged but not required. |
| Example |Soil Moisture|
| Format | [GCMD Keywords](https://forum.earthdata.nasa.gov/viewforum.php?f=7&&ServicesUsage=101&sid=89340eba8a64e8f66d8dcb392431831a) or Free Text |

| **Publication Date** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `datePublished` |
| Description | Specify a custom date or year when this dataset can be made publicly available. If this is not specified, it will default to the current date. |
| Example | 2019 or 2019-04-19 |
| Format | _YYYY or YYYY-MM-DD_ |

| **Usage Rights** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `license` |
| Description | Choose how you wish your data to be shared and reused. Creative Commons Attribution (CC BY 4.0) requires that the dataset be cited by anyone using the data. Creative Commons Public Domain (CC BY 1.0) dedicates the data to the public domain without restriction. When using the API, enter the URL for the selected CC BY license. |
| Example | Select Creative Commons Attribution (CC BY 4.0) or Creative Commons Public Domain (CC BY 1.0) |
| Format | Select choice |

| **Project** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `provider` |
| Description | Enter the name of the DOE project to associate with this dataset. If multiple projects were involved, enter the project that had the largest contribution to this dataset. When using the web form, you can choose from the drop down list as you begin to enter the project name. |
| Example | Next-Generation Ecosystem Experiments (NGEE) Tropics *PI: Jeffrey Chambers*|
| Format | Controlled List |

| **Funding Organizations** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `funder` |
| Description | List the organizations that funded the work. When using the web form, you can choose from the drop down list as you begin to enter the funding organization. |
| Example |*from dropdown list*]: U.S. DOE > Office of Science > Biological and Environmental Research (BER) |
| Format | Controlled List or Free Text |

| **DOE Contracts** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `award` |
| Description | List the numbers of any DOE contract under which the data in the package was funded. Enter "NONE" if no DOE funding applies. If the dataset is a result of a joint effort between two or more DOE Site/Facility Management Contractors, etc., additional DOE contract numbers may be entered.|
| Example |AC0205CH11231|
| Format | Controlled List or Free Text |

| **Related References** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `citation` |
| Description | Include the full citations and DOIs of datasets or publications associated with your dataset. These related materials allow users to learn more about the dataset, processing methods, or how the data were used. |
| Example |Somebody J. (2018), Sapflow and soil moisture coupling in the Amazon, Journal. doi: xx.xxxx|
| Format | Free Text |

| **Contact** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `editor` |
| Description |List the person who should be contacted by users seeking further information for the data. Only one contact is allowed. Including the ORCID of this individual is strongly encouraged.  |
| Example |First name, Last name, Organization, Email, ORCID (strongly encouraged)|
| Format | Free Text |

| **Creators** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `creator` |
| Description | Include the main researchers involved in producing the data such as authors, owners, originators, and principal investigators. List creators in the order they should appear in the dataset citation. One or more creators is required and including email addresses is highly encouraged. |
| Example |First name, Last name, Organization, Email, ORCID (not required for creators)|
| Format | Free Text |

| **Contributors** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `contributor` |
| Description | List any additional contributors involved in producing the data. These may include people who assisted in creating the dataset but are not considered authors. Contributors will not appear in the data citation. Including email addresses is highly encouraged.|
| Example |First name, Last name, Organization, Email, ORCID (not required for creators)|
| Format | Free Text |

| **Start Date** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `temporalCoverage` |
| Description | Earliest date of data collection included in the dataset. |
| Example|2017-04-16|
| Format | YYYY-MM-DD |

| **End Date** | **`optional`** | 
| :--- | :--- |
| JSON-LD Field | `temporalCoverage` |
| Description | Last date in data package. Leave blank if your dataset is open ended. | 
|Example | 2019-07-13|
| Format | YYYY-MM-DD |

| **Geographic Description** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `spatialCoverage/description` |
| Description | A short description of the location(s) where data was collected. This may include the location name, known identifiers if associated with a specific project (e.g. Ameriflux site name), and ecosystem type involved. Multiple geographic descriptions can be added if necessary. A complete geographic description will increase the findability of your dataset, as all terms entered are searchable through the data portal.|
| Example |Br-Ma2, Manaus, Brazil: ZF2 K34 Tower. Eddy covariance site established in 1999 on kilometer 34 of the ZF2 highway. It was later expanded into an atmospheric and soil sampling hub. It is a 1.5m x 2.5 m- section aluminum tower, 50 m tall, on a medium-sized plateau (Araujo et al., 2002).|
| Format | Free Text |

| **Bounding Box Coordinates** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `spatialCoverage` |
| Description | Latitude and Longitude of the location(s) this data represent in WGS84 decimal format. Enter only one coordinate pair for a single point and bounding box coordinates for non-point locations. Ensure coordinate accuracy before submitting your dataset. If the data location is better represented by a shape, you may also include a KML file in the file uploads. |
| Example |Northwest Coordinates `Lat Long`/Southeast Coordinates `Lat Long` |
| Format | Latitude and Longitude in WGS 84 decimal degrees |

| **Methods** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `measurementTechnique` |
| Description | Methods for a dataset should focus on all aspects of dataset production and should be thorough enough for your work to be reproduced. Include descriptions of the experimental design, laboratory and/or field collection methods (e.g. observations and/or devices used), source data for synthesis studies, data processing, and QA/QC procedures, and known issues or limitations of data where applicable. A complete methods section will improve findability of your data, as all text entered into methods will also be searchable for users through the data portal filters. *You may provide a citation for any methods used that were published previously, but methods related to data production must still be included.* |
| Example |An example of a complete methods section can be viewed at: Conlisk E ; Castanha C ; Germino M J ; Veblen T T ; Smith J M ; Kueppers L M (2017): Data from: "Declines in low-elevation subalpine tree populations outpace growth in high-elevation populations with warming". Subalpine and Alpine Species Range Shifts with Climate Change: Temperature and Soil Moisture Manipulations to Test Species and Population Responses. `doi:10.15485/1730950`|
| Format | Free Text |

