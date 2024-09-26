# Sample Catalogs

This repository holds some sample catalogs that you can use to explore the Bloomreach product and it's various features. 

Here is a sample curl request to upload a catalog to your account. Replace with your own `ACCOUNT_ID`, `CATALOG_NAME`, `ACCESS_TOKEN`. Once uploaded, you can see the job being processed on [Catalog Management](https://tools.bloomreach.com/navapp/discovery/catalogs/) on the Jobs page of the catalog you uploaded to

```bash
curl -v --request PUT \
     --url https://api.connect.bloomreach.com/dataconnect/api/v1/accounts/{INSERT_ACCOUNT_ID}/catalogs/{INSERT_CATALOG_NAME}/products \
     --header 'Content-Type: application/json-patch+jsonlines' \
     --header 'Authorization: {INSERT_ACCESS_TOKEN}' \
     --data-binary @./pacifichome_mini_en/pacifichome_mini_en.jsonl
```

## Related documentation
- [Catalog Management APIs Overview](https://documentation.bloomreach.com/discovery/reference/api-based-catalog-data-management)
- [Catalog management](https://documentation.bloomreach.com/discovery/docs/catalog-management)

## Related resources

- [Bloomreach SDK](https://documentation.bloomreach.com/discovery/docs/discovery-sdks)
- [Limitless Commerce UI Kit](https://bloomreach.github.io/limitless-ui-react)
- [Web Code Samples](https://documentation.bloomreach.com/discovery/docs/discovery-web-code-samples)
