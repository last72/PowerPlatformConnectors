# Airtable
Airtable is a cloud based spreadsheet-like service. V2 uses OAuth 2.0

## Publisher: Woong Choi

## Prerequisites
You need to have an Airtable account. You can [sign up](https://airtable.com/signup) for free.

## Supported Operations
### List Records
List records in the table.

### Create a Record
Create a record in a table.

### Retrieve a Record
Get a record details in a table.

### Delete a Record
Delete a record in a table.

### Update a Record
Update a record in a table.

## Set OAuth 2.0
[OAuth 2.0](https://airtable.com/developers/web/api/oauth-reference) is used for Airtable access. You need to [register integration](https://airtable.com/developers/web/guides/oauth-integrations) from [developers page](https://airtable.com/create/oauth).
Set redirect URL to https://global.consent.azure-apim.net/redirect

## Getting Started
Visit Airtable [REST API](https://airtable.com/developers/web/api/introduction) documentations page for further details. You may need to sign in to Airtable to view.

## Known Issues and Limitations
This connector cannot list bases as it require Airtable Metadata API. Further development is in plan for the API.

The response from the API is different for each table structure. You may need to use "Parse JSON" action to use the response to other action in Power Automate. It applies to "List Records", "Retrieve a Record", and "Update a Record" operation.

## Deployment Instructions
Inport the swagger file in target PowerApps environment.