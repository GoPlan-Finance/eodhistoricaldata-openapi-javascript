# EOD Historical Data Javascript/Typescript API Client

### [Click Here to see the current status and avalable endpoints](https://github.com/GoPlan-Finance/eodhistoricaldata-openapi)

## Installation
```bash
 # (we will publish to NPM later this month)
 npm i goplan-finance/eodhistoricaldata-openapi-js
 ```


## Example

**Typescript is also fully supported**, you will get full intellisense in both Javascript and Typescript.

```javascript
import * as EODApi from 'eodhistoricaldata-openapi'

const config = new EODApi.Configuration({
    apiKey : 'xxxxxxxxxxx',
})

const exchangesApi = new EODApi.ExchangesApi(this.config)

const response = await exchangesApi.listEchanges()

console.log(`We received ${response.data.length} exchanges`)
for (const exchange of response.data) {

    console.log(`${asset.Code} ${asset.Name}   (${asset.Country}  $(asset.Currency}`)
    assets.push({
        currency : asset.Currency,
        code     : asset.Code,
        country  : asset.Country,
        name     : asset.Name,
      })
}    
```


# Status

### [Click Here to see the current status and avalable endpoints](https://github.com/GoPlan-Finance/eodhistoricaldata-openapi)


# Issues & PRs 

If you find an issue, or want to add a new endpoint, please submit them directly to https://github.com/GoPlan-Finance/eodhistoricaldata-openapi repository


