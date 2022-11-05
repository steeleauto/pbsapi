<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://steeleauto.com/img/logo.png" width="400"></a></p>

# Marketing & Development
- **[Steele Auto](https://steeleauto.com/)**
- **[Steele All EV](https://allev.ca/)**
- **[Steele Advantage Financing](https://steeleadvantagefinancing.com/)**
- **[Your Way Auto](https://yourcaryourway.ca/)**
- **[Steele Wheels](https://steelewheels.ca/)**

## Steele Auto Group: API For PBS Systems
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
```json
{
    "token": "45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX"
}
```
*i.e Authorization Header*
```
Authorization Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX
```
- ### Create/Update Contact
##### Request Type: POST API endpoint: /api/dealboxx/pbs/ContactSave
##### Example: https://steeleauto.com/api/dealboxx/pbs/ContactSave
##### Headers: 
``` 
Authorization: Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX 
Accept: application/json
```
##### Request *(JSON)*:
```json
{
  "ContactInfo": {
    "Id": "7129/00000000-0000-0000-0000-000000000000",
    "ContactId": "00000000000000000000000000000000",
    "SerialNumber": "7129",
    "Code": "",
    "LastName": "",
    "FirstName": "",
    "Salutation": "",
    "MiddleName": "",
    "ContactName": "",
    "ApartmentNumber": "",
    "Address": "",
    "City": "",
    "County": "",
    "State": "",
    "ZipCode": "",
    "BusinessPhone": "",
    "HomePhone": "",
    "CellPhone": "",
    "BusinessPhoneRawReverse": "",
    "HomePhoneRawReverse": "",
    "CellPhoneRawReverse": "",
    "FaxNumber": "",
    "EmailAddress": "",
    "Notes": "",
    "CriticalMemo": "",
    "Gender": "",
    "DriverLicense": "",
    "PreferredContactMethods": [],
    "LastUpdate": "\/Date(-62135596800000-0000)\/",
    "CustomFields": [],
    "FleetType": "",
    "SalesRepRef": "00000000000000000000000000000000",
    "Language": "",
    "PayableAccount": "",
    "ReceivableAccount": "",
    "PrimaryImageRef": "00000000000000000000000000000000",
    "PayableAccounts": [],
    "ReceivableAccounts": [],
    "IsAPVendor": false,
    "IsARCustomer": false
  }
}
```
##### Response 
```json
{
  "Message": "Information processed successfully.",
  "ReferenceNumber": 200,
  "ReferenceId": "00000000000000000000000000000000",
  "WasSuccessful": true
}
```