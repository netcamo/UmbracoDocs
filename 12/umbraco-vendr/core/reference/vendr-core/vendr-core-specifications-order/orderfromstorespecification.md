---
title: OrderFromStoreSpecification
description: API reference for OrderFromStoreSpecification in Vendr, the eCommerce solution for Umbraco
---
## OrderFromStoreSpecification

```csharp
public class OrderFromStoreSpecification : IQuerySpecification<OrderReadOnly>, 
    ISpecification<OrderReadOnly>
```

**Inheritance**

* interface [IQuerySpecification&lt;!0&gt;](../../../vendr-common/vendr-common-specifications/iqueryspecification-1/)
* interface [ISpecification&lt;!0&gt;](../../../vendr-common/vendr-common-specifications/ispecification-1/)

**Namespace**
* [Vendr.Core.Specifications.Order](../)

### Constructors

#### OrderFromStoreSpecification

```csharp
public OrderFromStoreSpecification(Guid storeId)
```


### Properties

#### StoreId

```csharp
public Guid StoreId { get; }
```


### Methods

#### Accept

```csharp
public void Accept(IVisitor visitor)
```


---

#### IsSatisfiedBy

```csharp
public bool IsSatisfiedBy(OrderReadOnly item)
```


<!-- DO NOT EDIT: generated by xmldocmd for Vendr.Core.dll -->