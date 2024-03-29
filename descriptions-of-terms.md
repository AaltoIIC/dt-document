# Descriptions of terms

## Main terms

| Term | Subterms | Description | Assignment | Type |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| version  |  | The version of the digital twin document | mandatory | string |
| privacy  |  | The privacy of the digital twin | mandatory | string |
| dt-id  |  | The digital twin id | mandatory | string |
| name  |  | Name of the digital twin | mandatory | string |
| description  |  | The description of the document | mandatory | string |
| createdMachine  |  | The creation date of the digital twin document (machine-readable) | mandatory | string |
| createdHuman  |  | The creation date of the digital twin document (human-readable)| mandatory | string |
| modifiedMachine  |  | The modification date of the digital twin document (machine-readable) | optional | string |
| modifiedHuman  |  | The modification date of the digital twin document (human-readable)| optional | string |
| owner  |  | Owner of the physcial asset | optional |  |
| type |  | Field that tells what the object is used for | optional | string |
| contact  |  | The contact person of the digital twin | optional | string |
|   | name* | The name of the contact person | mandatory | string |
|   | email* | The email of the contact person | mandatory | string |
| location  |   | Location of the physcial asset | optional | string |
|   | streetAddress* | The street address of the location | mandatory | string |
|   | gpsCoordinates* | The gps coordinates of the location | mandatory | string |
| manufacturer  |  | The manufacturer of the physical twin | optional | string |
| apiGatewayAddress  |  | Address of the API gateway of the Data Link | optional | string |
| functions |  | A list of paths with parameters for API Gateway| optional | list |
| relations  |  | Relations to other digital twins | optional | string |
|   | id* | The id of the other digital twin | mandatory | string |
|   | relationType* | The relation type between the digital twins -> options: "parent", "sibling", "child" | mandatory | string |
| features  |  | The features that include information of the digital twin | optional | string |
|   | name*  | The name of the feature | mandatory | string |
|   | description*  | The description of the feature | mandatory | string |
|   | address | The internet address of the feature | optional | string |
|   | requirement*  | The requirement needed to access the feature | mandatory | string |
|   | documentation  | The internet (or other) address of the documentation of the feature | optional | string |
|   | keywords* | The keywords of the information that the feature contains | mandatory | string |
|   | custom** | A custom field that can be added to describe the feature | optional | string |

<br>
* mandatory subterm <br>
** any key-value pair is allowed
