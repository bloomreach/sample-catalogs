# Sample Catalogs

This repository holds some sample catalogs that you can use to explore the Bloomreach product and it's various features. 

Here is a sample curl request to upload a catalog to your account. Replace with your own `ACCOUNT_ID`, `CATALOG_NAME`, `ACCESS_TOKEN`. Once uploaded, you can see the job being processed on [Catalog Management](https://tools.bloomreach.com/navapp/discovery/catalogs/) on the Jobs page of the catalog you uploaded to

```bash
curl -v --request PUT \
     --url https://api.connect.bloomreach.com/dataconnect/api/v1/accounts/{INSERT_ACCOUNT_ID}/catalogs/{INSERT_CATALOG_NAME}/products \
     --header 'Content-Type: application/json-patch+jsonlines' \
     --header 'Authorization: {INSERT_ACCESS_TOKEN}' \
     --data-binary @./pacifichome_mini/pacifichome_mini.jsonl
```