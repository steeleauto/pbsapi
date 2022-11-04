# Steele Auto Group: API For PBS Systems
## Base URL: https://steeleauto.com
### Get Authentication Token
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
*Note: Please use response token in Authorization headers*
```
42|387phvqUIGxUDMV7J2K1zW1SxXXXXXXXXX
```
*i.e Authorization Header*
```
Authorization Bearer 42|387phvqUIGxUDMV7J2K1zW1SxXXXXXXXXX
```