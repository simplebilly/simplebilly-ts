
# Employee


## Properties

Name | Type
------------ | -------------
`address` | string
`backupEmployeeId` | string
`bic` | string
`city` | string
`country` | [CountryCode](CountryCode.md)
`createdAt` | Date
`dateOfBirth` | Date
`deletedAt` | Date
`departmentId` | string
`email` | string
`firstName` | string
`gender` | [Gender](Gender.md)
`hireDate` | Date
`hourlyCost` | string
`iban` | string
`id` | string
`jobTitle` | string
`lastLogin` | Date
`lastName` | string
`lastUpdated` | Date
`monthlySalary` | string
`phone` | string
`state` | string
`status` | [EmployeeStatus](EmployeeStatus.md)
`tenantId` | string
`updatedAt` | Date
`userId` | string
`weeklyHours` | string
`zip` | string

## Example

```typescript
import type { Employee } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "address": null,
  "backupEmployeeId": null,
  "bic": null,
  "city": null,
  "country": null,
  "createdAt": null,
  "dateOfBirth": null,
  "deletedAt": null,
  "departmentId": null,
  "email": null,
  "firstName": null,
  "gender": null,
  "hireDate": null,
  "hourlyCost": null,
  "iban": null,
  "id": null,
  "jobTitle": null,
  "lastLogin": null,
  "lastName": null,
  "lastUpdated": null,
  "monthlySalary": null,
  "phone": null,
  "state": null,
  "status": null,
  "tenantId": null,
  "updatedAt": null,
  "userId": null,
  "weeklyHours": null,
  "zip": null,
} satisfies Employee

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Employee
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


