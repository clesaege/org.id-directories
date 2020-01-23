* [AbstractOrganizationFactory](#abstractorganizationfactory)
  * [OrganizationCreated](#event-organizationcreated)
  * [OwnershipTransferred](#event-ownershiptransferred)
  * [create](#function-create)
  * [create](#function-create)
  * [createAndAddToDirectory](#function-createandaddtodirectory)
  * [createAndAddToDirectory](#function-createandaddtodirectory)
  * [createdOrganizations](#function-createdorganizations)
  * [createdOrganizationsIndex](#function-createdorganizationsindex)
  * [getCreatedOrganizations](#function-getcreatedorganizations)
  * [getCreatedOrganizationsLength](#function-getcreatedorganizationslength)
  * [owner](#function-owner)

# AbstractOrganizationFactory

## *event* OrganizationCreated

AbstractOrganizationFactory.OrganizationCreated(organization) `47b68893`

Arguments

| **type** | **name** | **description** |
|-|-|-|
| *address* | organization | indexed |

## *event* OwnershipTransferred

AbstractOrganizationFactory.OwnershipTransferred(previousOwner, newOwner) `8be0079c`

Arguments

| **type** | **name** | **description** |
|-|-|-|
| *address* | previousOwner | indexed |
| *address* | newOwner | indexed |


## *function* create

AbstractOrganizationFactory.create(orgJsonUri, orgJsonHash) `nonpayable` `3dee0c50`

> Creates new 0xORG smart contract

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *string* | orgJsonUri | Organization's data pointer |
| *bytes32* | orgJsonHash | Organization's data hash |

Outputs

| **type** | **name** | **description** |
|-|-|-|
| *address* |  | undefined |

## *function* create

AbstractOrganizationFactory.create(orgJsonUri, orgJsonHash, parentAddress, subsidiaryDirector) `nonpayable` `a6dd857e`

> Creates new subsidiary 0xORG smart contract

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *string* | orgJsonUri | Organization's data pointer |
| *bytes32* | orgJsonHash | Organization's data hash |
| *address* | parentAddress | Parent organization address |
| *address* | subsidiaryDirector | Subsidiary director address |

Outputs

| **type** | **name** | **description** |
|-|-|-|
| *address* |  | undefined |

## *function* createAndAddToDirectory

AbstractOrganizationFactory.createAndAddToDirectory(orgJsonUri, orgJsonHash, directory, parentAddress, subsidiaryDirector) `nonpayable` `00a5a6a3`

> Creates new subsidiary 0xORG smart contract and adds it to a segment directory in the same transaction

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *string* | orgJsonUri | Organization's data pointer |
| *bytes32* | orgJsonHash | Organization's data hash |
| *address* | directory | Segment directory address |
| *address* | parentAddress | Parent organization address |
| *address* | subsidiaryDirector | Subsidiary director address |

Outputs

| **type** | **name** | **description** |
|-|-|-|
| *address* |  | undefined |

## *function* createAndAddToDirectory

AbstractOrganizationFactory.createAndAddToDirectory(orgJsonUri, orgJsonHash, directory) `nonpayable` `af276209`

> Creates new 0xORG smart contract and adds it to a segment directory in the same transaction

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *string* | orgJsonUri | Organization's data pointer |
| *bytes32* | orgJsonHash | Organization's data hash |
| *address* | directory | Segment directory address |

Outputs

| **type** | **name** | **description** |
|-|-|-|
| *address* |  | undefined |

## *function* createdOrganizations

AbstractOrganizationFactory.createdOrganizations(index) `view` `9e356f4c`

> Returns organization address on `index` position.

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *uint256* | index | undefined |


## *function* createdOrganizationsIndex

AbstractOrganizationFactory.createdOrganizationsIndex(organization) `view` `0a1bd90b`

> Returns index of `organization`

Inputs

| **type** | **name** | **description** |
|-|-|-|
| *address* | organization | undefined |


## *function* getCreatedOrganizations

AbstractOrganizationFactory.getCreatedOrganizations() `view` `270ca0f0`

> Returns a list of created organizations.




## *function* getCreatedOrganizationsLength

AbstractOrganizationFactory.getCreatedOrganizationsLength() `view` `3db297e9`

> Returns number of created organizations.




## *function* owner

AbstractOrganizationFactory.owner() `view` `8da5cb5b`

> Returns the address of the current owner.




---