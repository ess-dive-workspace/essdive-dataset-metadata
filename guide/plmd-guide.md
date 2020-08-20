# Package-level metadata guide

This page provides guidelines and expectations for each metadata field for uploads to the ESS-DIVE repository. The JSON LD Field Names refer to vocabulary used for submission through our API.

For data packages submitted through our [Web Form](https://app.gitbook.com/@ess-dive/s/docs/~/drafts/-M-FyzcRvPLvBzU4v_IX/data-and-metadata-upload/complete-guide), use the "Online Submission Field" terms. Use the "JSON-LD" terms when submitting through our [API](https://app.gitbook.com/@ess-dive/s/docs/~/drafts/-M-FyzcRvPLvBzU4v_IX/data-and-metadata-upload/complete-guide).

| **Title** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `name` |
| Description | Include a brief title between 7-20 words long which contains relevant information such as the topic, geographic location, dates, and scale of data. If data is associated with a journal publication, the title may include journal name. Avoid unexplained acronyms or project-specific vocabulary. If there is an existing DOI for the data, use the same title. |
| Format | Free Text |

| **Existing DOI & Alternate Identifier** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `alternateName` |
| Description | If the data package has been previously published elsewhere, include a valid DOI or alternate identifier. Alternate identifiers provide pertinent information that can identify and locate the data set within your site's data management system. |
| Format | Not free text |

| **Abstract** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `alternateName` |
| Description | The abstract should include at least 100 words that describe the purpose and content of the data package. The abstract should be understandable to anyone who has not seen related manuscripts, include all necessary scientific context, contain no unexplained acronyms, and be written in complete sentences. |
| Format | Free Text |

| **Keywords** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `keywords` |
| Description | Enter at least three keywords that are different from words in the title to enable thematic searches. Use the Global Change Master Directory \(GCMD\) keywords where possible. When using the web form, you can choose from the dropdown list as you begin to enter a term. Or, write your own term where needed. You can also look up GCMD keywords using the link provided, particularly when using the API. |
| Format | [GCMD Keywords](https://gcmd.nasa.gov/search/Keywords.do#keywords) or Free Text |

| **Data Variables** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `variablesMeasured` |
| Description | Add variables to increase the findability of your dataset in searches. Select variable terms from GCMD controlled keywords where possible. |
| Format | [GCMD Keywords](https://gcmd.nasa.gov/search/Keywords.do#keywords) or Free Text |

| **Publication Date** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `datePublished` |
| Description | Specify a custom date or year when this data package can be made publicly available. If this is not specified, it will default to the current date. |
| Format | _YYYY or YYYY-MM-DD_ |

| **Usage Rights** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `license` |
| Description | Choose how you wish your data to be shared and reused. [Creative Commons Attribution \(CC BY 4.0\)](https://creativecommons.org/licenses/by/4.0/) requires that the data package be cited by anyone using the data. [Creative Commons Public Domain \(CC BY 1.0\)](https://creativecommons.org/publicdomain/zero/1.0/) dedicates the data to the public domain without restriction. When using the API, enter the URL for the selected CC BY license. |
| Format | Select choice |

| **Project** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `provider` |
| Description | Enter the name of the DOE project to associate with this data package. If multiple projects were involved, enter the project that had the largest contribution to this data package. When using the web form, you can choose from the drop down list as you begin to enter the project name. |
| Format | Controlled List **NEEDLINK** |

| **Funding Organizations** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `funder` |
| Description | List the organizations that funded the work. When using the web form, you can choose from the drop down list as you begin to enter the funding organization. |
| Format | Controlled List or Free Text |

| **DOE Contract Number** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `award` |
| Description | List the numbers of any DOE contract under which the data in the package was funded. Enter "NONE" if no DOE funding applies. If the data package is a result of a joint effort between two or more DOE Site/Facility Management Contractors, etc., additional DOE contract numbers may be entered. |
| Format | Controlled List or Free Text |

| **Contact** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `editor` |
| Description | Person who should be listed as the contact for the data package for the purposes of the DOI or for users seeking further information for the data. Only one contact is allowed. |
| Format | Free Text |

| **Creators** | **`required`** |
| :--- | :--- |
| JSON-LD Field | `creator` |
| Description | The main researchers involved in producing the data. These include authors, owners, originators and principal investigators who should be listed in the citation. One or more creators is required. If none are entered, you will be set as the creator of this document. List creators in the order they need to appear in the citation. |
| Format | Free Text |

| **Contributors** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `contributor` |
| Description | Additional contributors involved in producing the data. These could include people who assisted in creating the data package but wouldn't be considered authors for publication. |
| Format | Free Text |

| **Start Date** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `temporalCoverage` |
| Description | Earliest date in data package. |
| Format | YYYY-MM-DD |

| **End Date** | **`required`** |  |  |
| :--- | :--- | :--- | :--- |
| JSON-LD Field | `temporalCoverage` |  |  |
| Description | Last date in data package. Leave blank if your dataset is open ended. | YYYY-MM-DD | No |
| Format | YYYY-MM-DD |  |  |

| **Geographic Description** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `spatialCoverage/description` |
| Description | Known identifiers \(e.g. Ameriflux site name\), name, and short descriptions of the locations\(s\) where data was collected. |
| Format | Free Text |

| **Bounding Box Coordinates** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `spatialCoverage` |
| Description | Latitude and Longitude of the location\(s\) this data represents in WGS84 decimal format. Enter only one coordinate pair for a single point and bounding box coordinates for non-point locations. If the data is better represented by a shape, you may also include a KML file in the file uploads. |
| Format | Latitude and Longitude  in WGS 84 decimal degrees |

| **Related References** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `citation` |
| Description | Associated publications or data packages where users can learn more about the dataset, processing method, or how the data were used. Include the full citation with DOI. |
| Format | Free Text |

| **Methods** | **`optional`** |
| :--- | :--- |
| JSON-LD Field | `measurementTechnique` |
| Description | Information about the methods employed in collecting or generating a data set or other resource. These include descriptions of sampling or experimental procedures, data QA/QC, processing and synthesis. |
| Format | Free Text |

