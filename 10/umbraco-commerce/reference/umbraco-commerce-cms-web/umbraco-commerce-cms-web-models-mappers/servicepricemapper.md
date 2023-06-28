---
title: ServicePriceMapper
description: API reference for ServicePriceMapper in Umbraco Commerce
---
## ServicePriceMapper

```csharp
public static class ServicePriceMapper
```

**Namespace**
* [Umbraco.Commerce.Cms.Web.Models.Mappers](README.md)

### Methods

#### AllowedCountryRegionServicePrices

```csharp
public static IEnumerable<ServicePriceDto> AllowedCountryRegionServicePrices(
    IEnumerable<ServicePriceDto> prices, IEnumerable<AllowedCountryRegionDto> allowedCountryRegions)
```


---

#### ServicePriceCollectionToDtos

```csharp
public static List<ServicePriceDto> ServicePriceCollectionToDtos(
    IEnumerable<ServicePrice> collection)
```


---

#### ServicePriceDtosToCollection

```csharp
public static IEnumerable<ServicePrice> ServicePriceDtosToCollection(
    IEnumerable<ServicePriceDto> dtos)
```


---

#### ServicePriceDtoToEntity

```csharp
public static ServicePrice ServicePriceDtoToEntity(ServicePriceDto dto)
```


---

#### ServicePriceEntityToDto

```csharp
public static ServicePriceDto ServicePriceEntityToDto(ServicePrice entity)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Cms.Web.dll -->