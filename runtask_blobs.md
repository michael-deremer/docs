# Runtask blobs

## RPE Build
```
{
  "state_machine_input": {
    "inner_task_name": "Gcp.ComputeRegionalPortfolioEvaluationsBuild",
    "customer_id": "<insert>",
    "additional_context": {
      "gcp_billing_account_id": "<insert>"
    }
  }
}
```

## GPE Build
```
{
  "state_machine_input": {
    "dry_run": false,
    "customer_id": "<insert>",
    "inner_task_name": "Gcp.Ops.ComputeGlobalPortfolioEvaluationsBuild",
    "additional_context": {
      "gcp_billing_account_id": "<insert>"
    }
  }
}
```

## Google Seed purchases WI Generation
```
{
  "state_machine_input": {
    "inner_task_name": "Gcp.ResourceCommitSeedingWorkItems",
    "customer_id": "<insert>",
    "additional_context": {
      "gcp_billing_account_id": "insert",
      "billing_offering": "AutonomousDiscountManagementForGcpComputeEngine",
      "seed_start_date": "YYYY-MM-DD"
    }
  }
}
```

## Google Account Deactivation
** Always double check the id is actually for a customer we want to deactivate account for** 
```
{
  "state_machine_input": {
    "inner_task_name": "Gcp.Ops.DeactivateBillingAccount",
    "customer_id": "ae3bdaf0-3ab5-46bc-8a32-1fde8313afcf",
    "additional_context": {
      "gcp_billing_account_id": "00738a10-2dda-4301-ae7d-f9a0a9367b4b"
    }
  }
}
```
