# Corrections and Proposed Additions for the Book "Stylish F#" by Kit Eason, Apress, 2018

https://www.apress.com/us/book/9781484239995

This repo contains corrections and potential additions for the book "Stylish F". If you see a typo or code mistake, or would like to suggest additional or revised content, please submit a PR here. Changes will be incorporated in the next edition when possible.

---

## Corrections

#### Chatper 4, ppage 65

Is `unfold` really an example starting with nothing?

#### Chapter 4, page 93, Recommendations

*Currently reads:*

> I want the average of largest three

*Should read:*

> I want the average of **the** largest three

#### Chapter 5, page 100

*Currently reads:*

> ...keep updating it if it the...

*Should read:*

> ...keep updating it if the...

#### Chapter 6, page 142

"...as the real (government endorsed!) as one is..." -- delete the second "as".

#### Chapter 6, page 143, Listing 6-28

`Some s` is incorrectly indented.

#### Chapter 7, page 168

Worth pointing out that `Fable.Remoting` makes nice use of
records as interfaces.

Make the point that using interfaces rather than records-as-functions is an example of motivational transparency.

#### Chapter 8, page 196, Listing 8-11

*Currently reads:*

```fsharp
// Requires the version of ConsolePrompt from Listing 8-4
```

*Should read:*

```fsharp
// Requires the version of ConsolePrompt from Listing 8-11
```

#### Chapter 8, Page 202, "Interfaces"

Need to amend this section to reflect the fact that you can have parameter names in interface definitions.

#### Chapter 9, Page 241, Listing 9-14

The typographic quotes in the listing have incorrectly been replaced with neutral quotes.

#### Chapter 10, Page 267

Change "highly questionable, main wiring" to "highly questionable mains wiring".

#### Chapter 13, Page 359

Remove paragraph saying that it would now be a good time to rurun the code.

---

## Additions

#### Chapter 3 - Missing Data

- Add new section on `Option.orElse`.

#### Chapter 4 - Working Effectively with Collection Functions

- Add a cross reference between LINQ naming and F# name - e.g. SelectMany -> collect

#### Chapter 6 - Pattern Matching

- Add something about the `KeyValuePair` active pattern, especially when working with dictionaries/maps.

#### Chapter 10 - Asynchronous and Parallel Programming

- Add new section on `TaskBuilder.fs`: https://github.com/rspeele/TaskBuilder.fs/blob/master/TaskBuilder.fs

#### Type Providers

Consider adding a section on type providers.

- SQL
- CSV
- CSV versus CSVFile
- Sampling issues
- JSON

#### F# 4.6

##### Anonymous Record Types

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
