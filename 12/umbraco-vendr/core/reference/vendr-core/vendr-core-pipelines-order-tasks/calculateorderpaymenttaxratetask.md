---
title: CalculateOrderPaymentTaxRateTask
description: API reference for CalculateOrderPaymentTaxRateTask in Vendr, the eCommerce solution for Umbraco
---
## CalculateOrderPaymentTaxRateTask

```csharp
public class CalculateOrderPaymentTaxRateTask : 
    PipelineTaskWithTypedArgsBase<OrderCalculationPipelineArgs, OrderCalculation>
```

**Inheritance**

* class [PipelineTaskWithTypedArgsBase&lt;!0,!1&gt;](../../../vendr-common/vendr-common-pipelines/pipelinetaskwithtypedargsbase-2/)

**Namespace**
* [Vendr.Core.Pipelines.Order.Tasks](../)

### Constructors

#### CalculateOrderPaymentTaxRateTask

```csharp
public CalculateOrderPaymentTaxRateTask(IPaymentCalculator paymentCalculator)
```


### Methods

#### Execute

```csharp
public override PipelineResult<OrderCalculation> Execute(OrderCalculationPipelineArgs args)
```


<!-- DO NOT EDIT: generated by xmldocmd for Vendr.Core.dll -->