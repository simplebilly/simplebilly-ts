
# SubscriptionOverview

Tenant subscription overview for the billing page: current plan, status, period end, trial state, effective limits, current usage and feature flags. Backed by Paddle Billing webhook data written into `billing_info` + `tenants.plan`, and by the canonical plans in `crate::saasy::plans`.  JSON contract (camelCase, matches the frontend): `plan`, `planName`, `priceEur`, `status`, `currentPeriodEnd`, `manageUrl`, `trialEndsAt`, `isTrialing`, `limits:{maxUsers,maxInvoicesPerMonth,maxConnectors}`, `usage:{users,invoicesThisMonth,connectors,overageSeats}`, `features:{taxAutomations,fancyReports,erp}`.

## Properties

Name | Type
------------ | -------------
`currentPeriodEnd` | Date
`features` | [PlanFeatures](PlanFeatures.md)
`isTrialing` | boolean
`limits` | [PlanLimits](PlanLimits.md)
`manageUrl` | string
`plan` | string
`planName` | string
`priceEur` | number
`quantity` | number
`status` | string
`subscriptionId` | string
`trialEndsAt` | Date
`usage` | [UsageSnapshot](UsageSnapshot.md)

## Example

```typescript
import type { SubscriptionOverview } from '@simplebilly/api'

// TODO: Update the object below with actual values
const example = {
  "currentPeriodEnd": null,
  "features": null,
  "isTrialing": null,
  "limits": null,
  "manageUrl": null,
  "plan": null,
  "planName": null,
  "priceEur": null,
  "quantity": null,
  "status": null,
  "subscriptionId": null,
  "trialEndsAt": null,
  "usage": null,
} satisfies SubscriptionOverview

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SubscriptionOverview
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


