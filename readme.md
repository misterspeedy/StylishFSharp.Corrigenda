# Corrections and Proposed Additions for the Book "Stylish F#" by Kit Eason, Apress, 2018

https://www.apress.com/us/book/9781484239995

This repo contains corrections and potential additions for the book "Stylish F". If you see a typo or code mistake,
please submit a PR here. Changes will be incorporated in the next edition when possible.

---

## Corrections

#### Chapter 4, page 93, Recommendations

*Currently reads:*

> I want the average of largest three

*Should read:*

> I want the average of **the** largest three

#### Chapter 6, page 143, Listing 6-28

`Some s` is incorrectly indented.

#### Chapter 7, page 168

Worth pointing out that `Fable.Remoting` makes nice use of
records as interfaces.

#### Chapter 8, page 196, Listing 8-11

*Currently reads:*

```fsharp
// Requires the version of ConsolePrompt from Listing 8-4
```

*Should read:*

```fsharp
// Requires the version of ConsolePrompt from Listing 8-11
```
---

## Additions

##### Chapter 3 - Missing Data

- Add new section on `Option.orElse`.

##### Type Providers

Consider adding a section on type providers.

- SQL
- CSV
- CSV versus CSVFile
- Sampling issues
- JSON

##### F# 4.6

###### Anonymous Record Types

- Add new section to Chapter 7 to cover anonymous record types:


-- Instantiation


-- Consumption


-- Performance


-- Structs


-- Serialization


-- LINQ

- Amend existing commentary on long tuples in pipelines to include the
possibility of using anonymous record types.

See this for style comments: https://blogs.msdn.microsoft.com/dotnet/2019/01/24/announcing-f-4-6-preview/

###### ValueOption extensions

Delete/amend the para beginning *At the time of writing...* on p.55.


###### tryExactlyOne

Consider adding to Chapter 4.
