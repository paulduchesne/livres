# Livres
Identify primary-source book data, conformed to Wikidata entities and the Wikidata "Book data model" (https://www.wikidata.org/wiki/Wikidata:WikiProject_Books/Book_data_model).

## Primary source data

This project is an experiment in deriving claims around [work](https://www.wikidata.org/wiki/Q47461344) a [edition](https://www.wikidata.org/wiki/Q3331189) entities based on physical examination of an [individual copy of a book](https://www.wikidata.org/wiki/Q53731850). 

These collected claims are:

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
> - has published date (year) of 2009.

[^1]: This raises an interesting question, as [Q11827997](https://www.wikidata.org/wiki/Q11827997) is (at time of writing) already defined as a [literary work](https://www.wikidata.org/wiki/Q7725634), which is a subclass of [written work](https://www.wikidata.org/wiki/Q47461344). Good practice would be for OpenRefine to ignore this claim as redundant (ie, a more granular claim already exists).
[^2]: This claim already exists and should be ignored.
[^3]: Whether original titles should be treated as a monolingual label is an ongoing headache when mapping creative work labels to the excellent multilingual capabilities of Wikidata. 