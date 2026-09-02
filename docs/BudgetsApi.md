# BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**budgetsApi**](BudgetsApi.md#budgetsapi) | **GET** /api/v1/bookkeeping/budgets |  |
| [**upsertBudgetGoalApi**](BudgetsApi.md#upsertbudgetgoalapi) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} |  |



## budgetsApi

> BudgetErgebnis budgetsApi(year, month)



### Example

```ts
import {
  Configuration,
  BudgetsApi,
} from '@simplebilly/api';
import type { BudgetsApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BudgetsApi(config);

  const body = {
    // number
    year: 56,
    // number
    month: 56,
  } satisfies BudgetsApiRequest;

  try {
    const data = await api.budgetsApi(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **year** | `number` |  | [Defaults to `undefined`] |
| **month** | `number` |  | [Defaults to `undefined`] |

### Return type

[**BudgetErgebnis**](BudgetErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Monats-Budget + Prognose |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## upsertBudgetGoalApi

> Budget upsertBudgetGoalApi(category, budgetGoalRequest)



### Example

```ts
import {
  Configuration,
  BudgetsApi,
} from '@simplebilly/api';
import type { UpsertBudgetGoalApiRequest } from '@simplebilly/api';

async function example() {
  console.log("🚀 Testing @simplebilly/api SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer_token
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BudgetsApi(config);

  const body = {
    // string
    category: category_example,
    // BudgetGoalRequest
    budgetGoalRequest: ...,
  } satisfies UpsertBudgetGoalApiRequest;

  try {
    const data = await api.upsertBudgetGoalApi(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **category** | `string` |  | [Defaults to `undefined`] |
| **budgetGoalRequest** | [BudgetGoalRequest](BudgetGoalRequest.md) |  | |

### Return type

[**Budget**](Budget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Budget goal saved (upsert) |  -  |
| **400** | Negative goal |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

