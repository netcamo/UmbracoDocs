---
title: CalculateSubOrderLinePricesTask
description: API reference for CalculateSubOrderLinePricesTask in Vendr, the eCommerce solution for Umbraco
---
## CalculateSubOrderLinePricesTask

```csharp
public class CalculateSubOrderLinePricesTask : 
    SubOrderLinesCalculationPipelineBase<CalculateSubOrderLinePricesTask, CalculateOrderLinePricesPipeline>
```

**Inheritance**

* class [SubOrderLinesCalculationPipelineBase&lt;TSelf,TSubOrderLinePipeline&gt;](../suborderlinescalculationpipelinebase-2/)

**Namespace**
* [Vendr.Core.Pipelines.OrderLine.Tasks](../)

### Constructors

#### CalculateSubOrderLinePricesTask

```csharp
public CalculateSubOrderLinePricesTask(ILogger<CalculateSubOrderLinePricesTask> logger)
```


### Methods

#### AdditionalProcessing

```csharp
public override void AdditionalProcessing(OrderLineCalculationPipelineArgs parentPipelineArgs, 
    OrderLineCalculation orderLineCalculation)
```


<!-- DO NOT EDIT: generated by xmldocmd for Vendr.Core.dll -->