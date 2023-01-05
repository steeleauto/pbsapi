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
- ### Create/Update Vehicle
##### Request Type: POST API endpoint: /api/dealboxx/pbs/VehicleSave
##### Example: https://steeleauto.com/api/dealboxx/pbs/VehicleSave
##### Headers: 
``` 
Authorization: Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX 
Accept: application/json
```
##### Request *(JSON)*:
```json
{
  "VehicleInfo": {
    "Id": "7129/00000000-0000-0000-0000-000000000000",
    "VehicleId": "00000000000000000000000000000000",
    "SerialNumber": "7129",
    "StockNumber": "",
    "VIN": "",
    "LicenseNumber": "",
    "FleetNumber": "",
    "Status": "",
    "OwnerRef": "00000000000000000000000000000000",
    "ModelNumber": "",
    "Make": "",
    "Model": "",
    "Trim": "",
    "VehicleType": "",
    "Year": "",
    "Odometer": 0,
    "ExteriorColor": {
      "Code": "",
      "Description": ""
    },
    "InteriorColor": {
      "Code": "",
      "Description": ""
    },
    "Engine": "",
    "Cylinders": "",
    "Transmission": "",
    "DriveWheel": "",
    "Weight": 0,
    "LastServiceMileage": 0,
    "Lot": "",
    "LotDescription": "",
    "Category": "",
    "Options": [],
    "Refurbishments": [],
    "Order": {
      "Price": 0,
      "EstimatedCost": 0
    },
    "MSR": 0,
    "BaseMSR": 0,
    "Retail": 0,
    "InternetPrice": 0,
    "Lotpack": 0,
    "Holdback": 0,
    "InternetNotes": "",
    "Notes": "",
    "CriticalMemo": "",
    "LastUpdate": "\/Date(-62135596800000-0000)\/",
    "AppraisedValue": 0,
    "Warranties": [],
    "Freight": 0,
    "Air": 0,
    "Inventory": 0,
    "CustomFields": [],
    "FloorPlanCode": "",
    "FloorPlanAmount": 0,
    "Insurance": {
      "Company": "",
      "Policy": "",
      "ExpiryDate": "\/Date(-62135596800000-0000)\/",
      "AgentName": "",
      "AgentPhoneNumber": ""
    },
    "Body": "",
    "ShortVIN": "",
    "AdditionalDrivers": [],
    "OrderDetails": {},
    "PrimaryImageRef": "00000000000000000000000000000000",
    "Hold": {
      "VehicleRef": "00000000000000000000000000000000",
      "HoldFrom": "\/Date(-62135596800000-0000)\/",
      "HoldUntil": "\/Date(-62135596800000-0000)\/",
      "UserRef": "00000000000000000000000000000000",
      "ContactRef": "00000000000000000000000000000000"
    },
    "SalesDivision": 0,
    "TotalCost": 0,
    "BlueBookValue": 0,
    "VideoURL": "",
    "PDI": 0
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
- ### Create/Update Deal
##### Request Type: POST API endpoint: /api/dealboxx/pbs/DealSave
##### Example: https://steeleauto.com/api/dealboxx/pbs/DealSave
##### Headers: 
``` 
Authorization: Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX 
Accept: application/json
```
##### Request *(JSON)*:
```json
{
  "DealInfo": {
    "Id": "7129/00000000-0000-0000-0000-000000000000",
    "DealId": "00000000000000000000000000000000",
    "SerialNumber": "7129",
    "DealKey": "",
    "DealType": "",
    "UserRoles": [],
    "CreationDate": "\/Date(-62135596800000-0000)\/",
    "DeliveryStepsCompleted": [],
    "Conditions": "",
    "Status": "",
    "SaleType": "",
    "TaxCode": "",
    "Notes": "",
    "AmortizationTerm": 0,
    "PaymentTerm": 0,
    "PaymentTermMonths": 0,
    "PaymentsPerYear": 12,
    "Price": 0,
    "BuyerRef": "00000000000000000000000000000000",
    "CoBuyerRefs": [],
    "LastUpdate": "\/Date(-62135596800000-0000)\/",
    "Fees": [],
    "Accessories": [],
    "Warranties": [],
    "Protections": [],
    "Insurance": [],
    "Trades": [],
    "Rebates": [],
    "Allowances": [],
    "BackEndAllowances": [],
    "Adjustments": [],
    "Vehicles": [],
    "VehicleInsurance": {
      "Agent": "",
      "Address": "",
      "City": "",
      "Province": "",
      "PostalCode": "",
      "Phone": "",
      "Fax": "",
      "InsuranceCompany": "",
      "SaleNumber": "",
      "PolicyNumber": "",
      "PolicyEffective": "",
      "PolicyExpiry": "",
      "Collision": 0,
      "Comprehensive": 0,
      "Liability": 0
    },
    "CashInfo": {
      "MSRP": 0,
      "Taxes": [],
      "Deposit": 0,
      "DueOnDelivery": 0
    },
    "FinanceInfo": {
      "MSRP": 0,
      "Deposit": 0,
      "CashOnDelivery": 0,
      "Bank": "",
      "BankInfo": {
        "Code": "",
        "Name": "",
        "Address": "",
        "Phone": "",
        "Fax": "",
        "City": "",
        "State": "",
        "ZipCode": "",
        "BankNumber": ""
      },
      "Rate": 0,
      "EffectiveRate": 0,
      "PaymentsPerYear": 0,
      "PaymentTerm": 0,
      "PaymentTermMonths": 0,
      "AmortizationTerm": 0,
      "Balloon": 0,
      "BalanceToFinance": 0,
      "FinanceCharges": 0,
      "TotalBalanceDue": 0,
      "PaymentBase": 0,
      "PaymentTaxes": [],
      "Payment": 0,
      "Term": 0,
      "APR": 0
    },
    "LeaseInfo": {
      "MSRP": 0,
      "CapTaxes": [],
      "CapSettings": [],
      "CapCost": 0,
      "CashOnDelivery": 0,
      "CapReduction": 0,
      "NetLease": 0,
      "ResidualPercent": 0,
      "ResidualAmount": 0,
      "InceptionMilesAllowed": 0,
      "InceptionMileageRate": 0,
      "InceptionMileageIncluded": false,
      "MileageCategory": "",
      "MileageAllowed": 0,
      "MileageExpected": 0,
      "MileageRate": 0,
      "ExcessMileageRate": 0,
      "MileageCharges": 0,
      "ResidualNet": 0,
      "ResidualAdjustment": 0,
      "Depreciation": 0,
      "Bank": "",
      "BankInfo": {
        "Code": "",
        "Name": "",
        "Address": "",
        "Phone": "",
        "Fax": "",
        "City": "",
        "State": "",
        "ZipCode": "",
        "BankNumber": ""
      },
      "LeaseCalculationModel": "",
      "Rate": 0,
      "EffectiveRate": 0,
      "PaymentsPerYear": 0,
      "PaymentTerm": 0,
      "PaymentTermMonths": 0,
      "AmortizationTerm": 0,
      "PaymentBase": 0,
      "PaymentTaxes": [],
      "Payment": 0,
      "UpfrontTaxes": [],
      "SecurityDeposit": 0,
      "DriveOffLease": 0,
      "PayableOnDelivery": 0,
      "Term": 0,
      "APR": 0
    },
    "Gross": {
      "Reserve": {
        "Amount": 0,
        "BaseRate": 0,
        "MidRate": 0,
        "Factor": 0
      },
      "VehicleGross": 0,
      "AccessoryGross": 0,
      "FinanceGross": 0,
      "DealGross": 0,
      "Incentives": 0
    },
    "DealTags": [],
    "LeadRef": "",
    "LeadSource": "",
    "LeadType": "",
    "StatusInfo": [],
    "SystemStatus": "",
    "DealInterestType": "",
    "DealCommissions": 0,
    "DealActivityInfo": [],
    "CashOnDelivery": 0,
    "APR": 0
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
- ### Create/Update Repair Order
##### Request Type: POST API endpoint: /api/dealboxx/pbs/RepairOrderSave
##### Example: https://steeleauto.com/api/dealboxx/pbs/RepairOrderSave
##### Headers: 
``` 
Authorization: Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX 
Accept: application/json
```
##### Request *(JSON)*:
```json
{
  "RepairOrderInfo": {
    "Id": "7129/00000000-0000-0000-0000-000000000000",
    "RepairOrderId": "00000000000000000000000000000000",
    "SerialNumber": "7129",
    "RepairOrderNumber": 0,
    "DateOpened": "\/Date(-62135596800000-0000)\/",
    "ContactRef": "00000000000000000000000000000000",
    "VehicleRef": "00000000000000000000000000000000",
    "MileageIn": 0,
    "MileageOut": 0,
    "IsWaiter": false,
    "IsComeback": false,
    "Requests": [],
    "CustomerSummary": {
      "Labour": 0,
      "Parts": 0,
      "OilGas": 0,
      "SubletTow": 0,
      "Misc": 0,
      "Environment": 0,
      "ShopSupplies": 0,
      "Freight": 0,
      "WarrantyDeductible": 0,
      "Discount": 0,
      "SubTotal": 0,
      "Tax1": 0,
      "Tax2": 0,
      "InvoiceTotal": 0,
      "CustomerDeductible": 0,
      "GrandTotal": 0,
      "LabourDiscount": 0,
      "PartDiscount": 0,
      "ServiceFeeTotal": 0
    },
    "WarrantySummary": {
      "Labour": 0,
      "Parts": 0,
      "OilGas": 0,
      "SubletTow": 0,
      "Misc": 0,
      "Environment": 0,
      "ShopSupplies": 0,
      "Freight": 0,
      "WarrantyDeductible": 0,
      "Discount": 0,
      "SubTotal": 0,
      "Tax1": 0,
      "Tax2": 0,
      "InvoiceTotal": 0,
      "CustomerDeductible": 0,
      "GrandTotal": 0,
      "LabourDiscount": 0,
      "PartDiscount": 0,
      "ServiceFeeTotal": 0
    },
    "InternalSummary": {
      "Labour": 0,
      "Parts": 0,
      "OilGas": 0,
      "SubletTow": 0,
      "Misc": 0,
      "Environment": 0,
      "ShopSupplies": 0,
      "Freight": 0,
      "WarrantyDeductible": 0,
      "Discount": 0,
      "SubTotal": 0,
      "Tax1": 0,
      "Tax2": 0,
      "InvoiceTotal": 0,
      "CustomerDeductible": 0,
      "GrandTotal": 0,
      "LabourDiscount": 0,
      "PartDiscount": 0,
      "ServiceFeeTotal": 0
    },
    "MemoCustomerCopy": false,
    "AppointmentNumber": 0,
    "LastUpdate": "\/Date(-62135596800000-0000)\/",
    "IsHardCopyPrinted": true,
    "PendingRequests": [],
    "DeferredRequests": [],
    "CancelledRequests": [],
    "Priority": 0,
    "NotifyType": "",
    "VINInquiryPerformed": false,
    "SONote": ""
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
- ### Create/Update Service Appointment
##### Request Type: POST API endpoint: /api/dealboxx/pbs/AppointmentSave
##### Example: https://steeleauto.com/api/dealboxx/pbs/AppointmentSave
##### Headers:
``` 
Authorization: Bearer 45|BVFwfuSTTMjYpwuCin2OS2V8XXXXXXXXXX 
Accept: application/json
```
##### Request *(JSON)*:
```json
{
  "AppointmentInfo": {
    "Id": "7129/00000000-0000-0000-0000-000000000000",
    "AppointmentId": "00000000000000000000000000000000",
    "SerialNumber": "7129",
    "AppointmentNumber": 0,
    "RawAppointmentNumber": "",
    "Shop": "",
    "Advisor": "",
    "BookingUser": "",
    "Transportation": "",
    "ContactRef": "00000000000000000000000000000000",
    "VehicleRef": "00000000000000000000000000000000",
    "MileageIn": 0,
    "IsComeback": false,
    "IsWaiter": false,
    "AppointmentTime": "\/Date(-62135596800000-0000)\/",
    "PickupTime": "\/Date(-62135596800000-0000)\/",
    "RequestLines": [
      {
        "AppointmentRequestRef": "00000000000000000000000000000000",
        "AppointmentRequestId": -1,
        "CSR": "",
        "Skill": "",
        "RequestCode": "",
        "RequestDescription": "",
        "AllowedHours": 0,
        "EstimateLabour": 0,
        "EstimateParts": 0,
        "PartsLines": [
          {
            "AppointmentPartsLineRef": "00000000000000000000000000000000",
            "AppointmentPartsLineId": -1,
            "CSR": "",
            "PartNumber": "",
            "PartDescription": "",
            "Requested": 0,
            "Shipped": 0,
            "Ordered": 0,
            "PriceCode": "",
            "Cost": 0,
            "UnitPrice": 0,
            "ExtendedPrice": 0,
            "IsPartsKit": false,
            "PartsKitName": "",
            "BIN": "",
            "IsTransferred": false
          }
        ],
        "LabourOpDescription": "",
        "PayType": "",
        "Tech": "",
        "Status": ""
      }
    ],
    "LastUpdate": "\/Date(-62135596800000-0000)\/",
    "Status": "",
    "Notes": "",
    "Source": "",
    "PendingRequest": false,
    "CheckedIn": false,
    "LeadRef": "",
    "NotifyType": "",
    "Tag": ""
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