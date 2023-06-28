---
title: ReadOnlyTranslatedValue<T>
description: API reference for ReadOnlyTranslatedValue<T> in Umbraco Commerce
---
## ReadOnlyTranslatedValue&lt;T&gt;

```csharp
public class ReadOnlyTranslatedValue<T> : ValueObjectBase
```

**Inheritance**

* class [ValueObjectBase](../../umbraco-commerce-common/umbraco-commerce-common-models/valueobjectbase.md)

**Namespace**
* [Umbraco.Commerce.Core.Models](README.md)

### Indexers

#### ReadOnlyTranslatedValue&lt;T&gt;

```csharp
public T this[string languageIsoCode] { get; }
```


### Methods

#### DeepClone

```csharp
public override object DeepClone()
```


---

#### GetDefaultValue

```csharp
public T GetDefaultValue()
```


---

#### GetTranslatedValues

```csharp
public IReadOnlyDictionary<string, T> GetTranslatedValues()
```


---

#### GetValue

```csharp
public T GetValue(string languageIsoCode, bool fallbackToDefault = true)
```


---

#### HasValue

```csharp
public bool HasValue(string languageIsoCode)
```


---

#### ToString

```csharp
public override string ToString()
```


---

#### TryGetValue

```csharp
public bool TryGetValue(string languageIsoCode, out T value)
```


### Operators

#### ReadOnlyTranslatedValue&lt;T&gt; Implicit

```csharp
public static implicit operator T(ReadOnlyTranslatedValue<T> value)
```


<!-- DO NOT EDIT: generated by xmldocmd for Umbraco.Commerce.Core.dll -->