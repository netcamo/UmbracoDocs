---
title: GiftCardEditDto
description: API reference for GiftCardEditDto in Vendr, the eCommerce solution for Umbraco
---
## GiftCardEditDto

```csharp
public class GiftCardEditDto : GiftCardDto, IHasPath, INotificationModel
```

**Inheritance**

* class [GiftCardDto](../giftcarddto/)
* interface [IHasPath](../ihaspath/)

**Namespace**
* [Vendr.Umbraco.Web.Models](../)

### Constructors

#### GiftCardEditDto

The default constructor.

```csharp
public GiftCardEditDto()
```


### Properties

#### Notifications

```csharp
public List<BackOfficeNotification> Notifications { get; set; }
```


---

#### Path

```csharp
public List<string> Path { get; set; }
```


<!-- DO NOT EDIT: generated by xmldocmd for Vendr.Umbraco.Web.dll -->