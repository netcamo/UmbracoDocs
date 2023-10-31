---
title: ValidateGiftCardCurrencyChange
description: API reference for ValidateGiftCardCurrencyChange in Umbraco Commerce
---
## ValidateGiftCardCurrencyChange

```csharp
public class ValidateGiftCardCurrencyChange : ValidationEventBase
```

**Inheritance**

* Class [ValidationEventBase](../../umbraco-commerce-common/umbraco-commerce-common-events/validationeventbase.md)

**Namespace**
* [Umbraco.Commerce.Core.Events.Validation](README.md)

### Constructors

#### ValidateGiftCardCurrencyChange

```csharp
public ValidateGiftCardCurrencyChange(GiftCardReadOnly giftCard, ChangingValue<Guid> currencyId)
```


### Properties

#### CurrencyId

```csharp
public ChangingValue<Guid> CurrencyId { get; }
```


---

#### GiftCard

```csharp
public GiftCardReadOnly GiftCard { get; }
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Core.dll -->