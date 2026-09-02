
# EmployeeCreate


## Properties

Name | Type
------------ | -------------
`address` | string
`backupEmployeeId` | string
`bic` | string
`city` | string
`country` | [CountryCode](CountryCode.md)
`dateOfBirth` | Date
`departmentId` | string
`email` | string
`firstName` | string
`gender` | [Gender](Gender.md)
`hireDate` | Date
`hourlyCost` | string
`iban` | string
`jobTitle` | string
`lastLogin` | Date
`lastName` | string
`lastUpdated` | Date
`monthlySalary` | string
`phone` | string
`state` | string
`status` | [EmployeeStatus](EmployeeStatus.md)
`userId` | string
`weeklyHours` | string
`zip` | string

## Example

```typescript
import type { EmployeeCreate } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "backupEmployeeId": null,
  "bic": null,
  "city": null,
  "country": null,
  "dateOfBirth": null,
  "departmentId": null,
  "email": null,
  "firstName": null,
  "gender": null,
  "hireDate": null,
  "hourlyCost": null,
  "iban": null,
  "jobTitle": null,
  "lastLogin": null,
  "lastName": null,
  "lastUpdated": null,
  "monthlySalary": null,
  "phone": null,
  "state": null,
  "status": null,
  "userId": null,
  "weeklyHours": null,
  "zip": null,
} satisfies EmployeeCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as EmployeeCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


