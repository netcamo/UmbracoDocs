---
title: CalculateOrderLineTotalPriceAdjustmentTask
description: API reference for CalculateOrderLineTotalPriceAdjustmentTask in Umbraco Commerce
---
## CalculateOrderLineTotalPriceAdjustmentTask

```csharp
public class CalculateOrderLineTotalPriceAdjustmentTask : 
    PipelineTaskWithTypedArgsBase<OrderLineCalculationPipelineArgs, OrderLineCalculation>
```

**Inheritance**

* class [PipelineTaskWithTypedArgsBase&lt;!0,!1&gt;](../../umbraco-commerce-common/umbraco-commerce-common-pipelines/pipelinetaskwithtypedargsbase-2.md)

**Namespace**
* [Umbraco.Commerce.Core.Pipelines.OrderLine.Tasks](README.md)

### Constructors

#### CalculateOrderLineTotalPriceAdjustmentTask

The default constructor.

```csharp
public CalculateOrderLineTotalPriceAdjustmentTask()
```


### Methods

#### Execute

```csharp
public override PipelineResult<OrderLineCalculation> Execute(OrderLineCalculationPipelineArgs args)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Core.dll -->