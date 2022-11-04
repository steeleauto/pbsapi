# Steele Auto Group: API For PBS Systems
## Base URL: https://steeleauto.com
- ### Get Authentication Token
*Please contact development team to get your account and authorization to use all endpoints*
##### Request Type: POST API endpoint: /api/dealboxx/login/token
##### Example: https://steeleauto.com/api/dealboxx/login/token
##### Request:
```json
{
    "email":"username@steeleauto.com",
    "password":"PROVIDED_PASSWORD_FROM_OUR_SYSTEM"
}
```
##### Response: 
*Note: Please use response token in Authorization headers for all endpoints mentioned in this wiki page*
```
42|387phvqUIGxUDMV7J2K1zW1SxXXXXXXXXX
```
*i.e Authorization Header*
```
Authorization Bearer 42|387phvqUIGxUDMV7J2K1zW1SxXXXXXXXXX
```
- ### Create/Update Contact
##### Request Type: POST API endpoint: /api/dealboxx/pbs/contact
##### Example: https://steeleauto.com/api/dealboxx/pbs/contact
##### Headers: 
``` Authorization Bearer 42|387phvqUIGxUDMV7J2K1zW1SxXXXXXXXXX ```
##### Request *(JSON)*:
```json
{
  "SerialNumber": "Numeric", 
  "Code": null, 
  "ContactId":"STRING | REQUIRED",
  "Salutation": null,
  "ContactName": null,
  "StatusName": null,
  "FullName": null,
  "FirstName": null,
  "MiddleName": null,
  "LastName": null,
  "ApartmentNumber": null,
  "Address": null,
  "City": null,
  "State": null,
  "ZipCode": null,
  "BusinessPhone": null,
  "HomePhone": null,
  "CellPhone": null,
  "FaxNumber": null,
  "EmailAddress": null,
  "BirthDate": null,
  "Gender": null,
  "DriverLicense": null,
  "CanEmail": null,
  "CanTextMessage": null,
  "CanPhone": null,
  "CanLetter": null,
  "CriticalMemo": null,
  "SalesRepRef": null,
}
```
##### Response 
```json
{
    "message": "Information processed successfully.",
    "code": 200,
    "data": {
        "ContactId": "00001f0ba6e54d5a8953aXXXXXXXX"
    },
    "success": true
}
```