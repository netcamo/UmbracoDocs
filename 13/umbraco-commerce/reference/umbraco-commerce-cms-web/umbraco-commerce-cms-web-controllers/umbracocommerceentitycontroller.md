---
title: UmbracoCommerceEntityController
description: API reference for UmbracoCommerceEntityController in Umbraco Commerce
---
## UmbracoCommerceEntityController

```csharp
public class UmbracoCommerceEntityController : UmbracoCommerceAuthorizedJsonControllerBase
```

**Inheritance**

* Class [UmbracoCommerceAuthorizedJsonControllerBase](umbracocommerceauthorizedjsoncontrollerbase.md)

**Namespace**
* [Umbraco.Commerce.Cms.Web.Controllers](README.md)

### Constructors

#### UmbracoCommerceEntityController

```csharp
public UmbracoCommerceEntityController(IBackOfficeSecurityAccessor backOfficeSecurityAccesor, 
    UmbracoCommerceContext ctx)
```


### Methods

#### DeleteEntity

```csharp
public IActionResult DeleteEntity(string entityType, Guid entityId)
```


---

#### GetEntities

```csharp
public IActionResult GetEntities(string entityType, Guid? storeId = default(Guid?), 
    Guid? parentId = default(Guid?))
```


---

#### GetEntity

```csharp
public IActionResult GetEntity(string entityType, Guid entityId)
```


---

#### GetStoreByEntityId

```csharp
public IActionResult GetStoreByEntityId(string entityType, Guid entityId)
```


---

#### SortEntities

```csharp
public IActionResult SortEntities(SortEntitiesPostDto model)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Cms.Web.dll -->