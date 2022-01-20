# Livres
- identify primary source book data.
- conform to Wikidata entities and the Wikidata "Book data model" (https://www.wikidata.org/wiki/Wikidata:WikiProject_Books/Book_data_model).
- submit work and edition data to Wikidata via OpenRefine.
- declare exemplar level data as self-hosted RDF.

## Primary source data

This project is an experiment in deriving claims for [work](https://www.wikidata.org/wiki/Q47461344), [edition](https://www.wikidata.org/wiki/Q3331189) and [exemplar](https://www.wikidata.org/wiki/Q53731850) entities based on physical examination of an [individual copy of a book](https://www.wikidata.org/wiki/Q53731850), in this example [Drive Your Plow Over the Bones of the Dead](https://www.wikidata.org/wiki/Q11827997). Work and edition data can be pushed to Wikidata as sufficently notable, while data related to the physical object can be shared as personal linked open data.

Collected claims are:

> Written Work (Q11827997)
> - is an instance of [written work](https://www.wikidata.org/wiki/Q47461344)[^1].
> - is written by [Olga Tokarczuk](https://www.wikidata.org/wiki/Q254032)[^2].
>
> First Edition (create)
> - is an instance of [version, edition, or translation](https://www.wikidata.org/wiki/Q3331189).
> - is in language [Polish](https://www.wikidata.org/wiki/Q809).
> - has title "Prowadź swój pług przez kości umarłych".
> - has label "Prowadź swój pług przez kości umarłych"[^3].
> - has publisher [Wydawnictwo Literackie](https://www.wikidata.org/wiki/Q3570203).
> - has published year of 2009.
> - edition of [Prowadź swój pług przez kości umarłych](https://www.wikidata.org/wiki/Q11827997).
> - description is "2009 Polish edition of written work by Olga Tokarczuk".
>
> Exemplar Edition (create)
> - is an instance of [version, edition, or translation](https://www.wikidata.org/wiki/Q3331189).
> - is in language [English](https://www.wikidata.org/wiki/Q1860).
> - has title "Drive Your Plow Over the Bones of the Dead".
> - has label "Drive Your Plow Over the Bones of the Dead".
> - is translated by [Antonia Lloyd-Jones](https://www.wikidata.org/wiki/Q61944439).
> - has publisher [Text Publishing](https://www.wikidata.org/wiki/Q17056193).
> - has published year of 2018.
> - has 247 pages[^4].
> - has an isbn of 9781925773088.
> - edition of [Prowadź swój pług przez kości umarłych](https://www.wikidata.org/wiki/Q11827997).
> - description is "2018 English edition of written work by Olga Tokarczuk".

## Merge issues

While the book model advocates for a multi-tier data model, this does intitiate the co-existence of a number of similarly named entities with possible data claim overlaps. This makes these items especially vulnerable  to an incorrect merge, either due to a badly configured bot, or a user not familiar with the model. 

A mitigating strategy would be to require editors of specific knowledge areas (in this case, literature) to gain some form of authentication to demonstrate that they understand the relevant data model.

[^1]: This raises an interesting question, as [Drive Your Plow Over the Bones of the Dead](https://www.wikidata.org/wiki/Q11827997) is (at time of writing) already defined as a [literary work](https://www.wikidata.org/wiki/Q7725634), which is a subclass of [written work](https://www.wikidata.org/wiki/Q47461344). Good practice would be for OpenRefine to ignore this claim as redundant (ie, a more granular claim already exists).
[^2]: This claim already exists and should be ignored.
[^3]: Whether a title of a creative work should be treated as monolingual for the work and edition-level labels is a major source of confusion. In theory, a literal translation of the original title into other languages would be most easily applicable, but this would cause practical problems when the work is well known in the other language by a completely different title (eg "Män som hatar kvinnor" translates literally to "Men Who Hate Women", not "The Girl with the Dragon Tattoo"). A further (although less common) issue is if the country has chosen to rename the film, but in the original language (eg the 2008 Mike Leigh film "Happy-Go-Lucky", released in France as "Be Happy").
[^4]: Not including unnumbered pages.