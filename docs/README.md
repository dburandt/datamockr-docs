# Datamockr API Reference

## Data Endpoint

> Retrieve an array of mock data

`GET /data?fieldType={fieldType}&size={size}`

```js
# example response to /data?fieldType=city&size=10
{
    "data": [
        'Toronto',
        'Wellington',
        'Miami',
        'Sydney',
        'Ulicesland',
        'Marcmouth',
        'Koelpinton',
        'London',
        'Edmonton',
        'Sherwood Park'
    ]
}
```

## Query Parameters

### fieldType

> The type of mock data to return

- Required: true
- Specs
  - String
  - See [fieldType possible values](#fieldType-possible-values)

### size

> The amount of mock data to return

- Required: true
- Specs
  - Integer
  - Must be less than (<) 1000

## fieldType possible values

### address

- zipCode
- city
- cityPrefix
- citySuffix
- streetName
- streetAddress
- streetSuffix
- streetPrefix
- secondaryAddress
- county
- country
- countryCode
- state
- stateAbbr
- latitude
- longitude
- direction
- cardinalDirection
- ordinalDirection
- nearbyGPSCoordinate
- timeZone

### commerce

- color
- department
- productName
- price
- productAdjective
- productMaterial
- product
- productDescription

### company

- companyName
- companySuffix
- catchPhrase
- bs
- catchPhraseAdjective
- catchPhraseDescriptor
- catchPhraseNoun
- bsAdjective
- bsBuzz
- bsNoun

### internet

- avatar
- email
- userName
- protocol
- url
- domainName
- domainSuffix
- domainWord
- ip
- ipv6
- userAgent
- mac
- password

### name

- fullName
- firstName
- lastName
- jobTitle
- prefix
- suffix
- title
- jobDescriptor
- jobArea
- jobType

### phone

- phoneNumber
- phoneNumberFormat
- phoneFormats
