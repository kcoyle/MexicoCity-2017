# Creating the Catalog, Before and After FRBR

by Karen Coyle

Talk given at *Encuentro di Catalogacion y Metadatos*; Universidad Nacional autonoma de Mexico; September 12, 2017

License: CC-BY (Feel free to re-use, translate, transform, but please given credit to the source, this document.)

## Introduction

There is a great deal of talk today about the future of the library catalog. 
There is also ongoing work on developing a "next generation" library bibliographic data format, 
possibly based on the model presented by the IFLA study group on the Functional Requirements for Bibliographic Records.  
There is a tendency, however, to treat the current state of data and catalogs as a starting point. 
The historical context is, however, much richer.

The history that we need to confront is long and complex. 
In terms of technology, you can date library catalogs back to the times of clay tablets and to tags 
affixed to the ends of scrolls in Greek and Roman times. 
Technological progress led to the use of book catalogs, paper slips, and eventually cards. 
In modern times the catalog technology moved from physical cards to a virtual catalog on computer and managed by a database system. 
In progress today is a transition from closed database systems to the use of the Web of data and the World Wide Web Consortium's 
Resource Description Framework (RDF) . 
 
We also need to consider how information itself has changed over time, from the first written symbols to virtual reality. 
And finally there is the lengthy history of libraries and their functions over the milennia of reccorded history.

Libraries have been innovators or organizational technology, although they shared their innovation with other professions with similar needs.
The move from book catalogs to cards in the late 19th century coincided with a move from ledger books to office filing systems within business ventures of the same time period.[Krajewski]
If we look, however, at the time line of information technology over the 20th century and into the 21st, we see library technology falling behind the general technology evolution.

[diagram]

Libraries moved to automated printing of cards in the very early days of computer technology, made possible by the development of an innovative record format for the card data, MAchine Readable Cataloging (MARC), in the mid-1960's. Not long after that, around 1980, that data was used for the first time to create library catalogs online, accessible first at terminals in the library and eventually from any networked point. Since that time library catalogs have gained features, such as federated searching of library holdings and journal article metadata. Yet the main technology remains the same, rooted in techniques from three or more decades past. 

During this same time, computer technology has made some significant changes; changes that are not reflected in library catalogs nor library information technology. At the time that the MARC record was first being used to print cards business applications were making use of database management systems that allowed them to store, search and modify text. Major innovations took place in database storage and techniques as well as data design and programming, such as relational database systems and object-oriented technology. After 1990 the emphasis of data sharing was around the technology of the World Wide Web and HTML, and indeed library catalogs did begin to deliver their data over the Internet within Web browsers. Documents and some data began to be coded in the eXtensible Markup Language (XML). An XML version fo the MARC record was devleoped, but it was no more than a new serialization of original MARC record - it provided no innovation in terms of data model or format. By the year 2000 the next generation of data models, RDF, was under development as the newest information technology, and the decades from 2000 to today, 2017, have shown an interest in created an open, linked information environment over the Web using RDF as its underlying abstract model.

Looking at the relative timelines, those of the overall information technology space and that of the library technology space, it becomes clear that libraries have failed to make the same changes that were happening in the other communities making use of computing. The reasons behind this are undoubtedly many, from issues of budget limitations, institutional conservatism, and the historicity of the library mission. 
I want to focus on one point that I see as a factor, and that is the transition from the card catalog to the online catalog. I can speak authoritatively about this because I must shoulder some of the blame for any errors made during this transition, as I was one of the people who designed and developed the University of California's online catalog. 

## Catalogs Past

A brief history of early catalogs and their designs can help us understand better how we missed some important clues about our own data when we moved from cards to computers.

Early catalogs, at least the ones that begin to resemble the catalogs that we use today, were book catalogs.

[picture]

Important aspects of the data for book catalogs was the conservation of space - thus the use of very brief bibliographic descriptions - and the use of alphabetically arranged headings under which to file those descriptions. The headings were generally the names of authors, and sometimes also titles and subjects, but always quite brief. 

An interesting version of a card system was developed in the late 1800's by Italian printer Natale Battezzati. His cards were reprints of the title page of the book with headings (author, subject) printed on the edges. The card itself could have quite a bit of information including table of contents (if there was room for this) and a summary. These cards allowed book sellers to create a merged catalog of the offerings of multiple printing houses, and hopefully to increase sales. Melvil Dewey cited this card system as an inspiration for the library card catalog.

[picture]

Because early library card catalogs were either hand-written or typed, it wasn't possible to include much information on the cards. In fact, many catalogs had separate cards for the headings and the bibliographic description, such that the cards with bibliographic data were filed after the header cards. 

[picture]

The headings and the bibliographic data were brought together, similar to Battezzati's scheme, only when cards were being printed. Like Battezzati's cards, the printed catalog cards each contained all of the detail about the resource, with headings written or typed at the top of the cards for filing in the catalog. The cards produced by the Library of Congress, and sold to libraries throughout the United States, also contained at the bottom the headings that LC had assigned to the resource. This served as an inventory of headings for each item, and also allowed other libraries to follow LC's practice.

[picture]

When the MARC format was developed in the 1960's, it was designed to drive computerized printing presses that would print the cards. One requirement was that the cards printed from MARC records had to look exactly like the cards that had been printed before using a type-setting process. The MARC record became a "unit record" containing all of the information that would be needed to print the cards, including the headings. 

[picture]

Like the catalogs that preceded it, the card catalog was a catalog of headings, and under those headings one would find the books or other resources owned by the library. In a sense, the card catalog was an index of the library. Each book appeared once on the shelf but was entered multiple times in the catalog, the headings spread out across the alphabetical order of the catalog. This was a very different order from the order of items on the shelf, and the catalog was considered necessary as a finding aid for users of the library.

The nature of the catalog was captured in the cataloging concept of "collocation" - that is, the locating of similar topics or names in close proximity within the alphabetical list. Once a user found an entry point in the alphabetical order, she could navigate forward or backward in the alphabetical listing. Because the alphabet is not itself a subject classification, the user would at some point navigate beyond their desired topic, at which point that catalog search would end.

[picture]

## From Cards to Computers

In the early 1980's we had the means to create a computerized catalog: we had MARC records that had been selected by libraries to have cards printed by OCLC, we had computers, and we had at least the promise of widespread networks for delivering the catalog to the libraries and their users. From today's perspective, it would be logical to assume that libraries moved from card catalogs to online catalogs as a way to improve the catalog for the user. That wasn't, however, the prime motivation.

For a large library, the card catalog was also very large. A library of one million items would have a card catalog that had from five to ten million cards. The catalog furniture was bulky and expensive, often taking up whole rooms in the library. But it was the cards themselves that were the problem. Ironically, the use of computing to print cards, and the ease with which libraries could order card sets through services like OCLC, meant that libraries were producing cards faster than they could file them. It was this final step, the filing of cards, that could not be automated.

In the late 1970's, when I began working on the University of California library automation program, the larger libraries in the system, such as Berkeley and Los Angeles, were unable to keep up with the filing of cards. At any given time these libraries were running 100,000-150,000 cards behind in their filing. That mean that a book was cataloged and placed on the shelf some three months before the book was entered into the catalog. This was clearly not acceptable for a research library. The computer catalog essentially automated filing, the final step in the catalog creation process. Except that it didn't file. And that's where the story gets interesting.

## MARC in a Database

MARC was developed for card printing, not for database storage. At the time that the first online catalogs were being developed, the common database management system was a relational database, which assumed that the data was organized into entities and relations. MARC is not, and therefore the conventional database design was one which stored the data in the MARC records as a single whole and developed access to the bibliographic record through keyword indexes. While the bibliographic data was itself unchanged from the card catalog era, the overall effect of this database design gave quite different results.

[slide]

Where the alphabetical browse through left-anchored headings provided some context for the user, the search in the database was like a black box - the user input a query and was shown a list of bibliographic records, but how the query terms caused the particular retrievals was hidden inside the functions of the database management system. The catalog had lost the contextual clues that librarians had created through the heading system.

As an example, the search above for cat breeds, using the Library of Congress catalog, returns many thousands of works which are presented to the user as brief bibliographic displays. These retrieved items are not in the order that they would be in the card catalog, which would be the order by the subject heading beginning "cat breeds." 

[picture]

In fact, if you look at these records in a detailed view, you see that the order is not by subject:

1. Cat breeds
2. Cat breeds
3. Cat breeds -- History
4. Cat breeds -- Handbooks, manuals, etc.
5. Cat breeds
6. Cat breeds -- Thailand

etc

The intention of the cataloging rules is to facilitate a display that takes advantage of the context provided by the headings. In fact, cataloging staff would have wanted a display that looks more like this:

<pre>
Cat breeds
	Arco book of cats / by Grace Pond
	Champion cats of the world / by Catherine Ing
	…
Cat breeds – Handbooks, manuals, etc.
	The complete cat owner's manual / Susie Page
	…
Cat breeds – History
	Fifty years of pedigree cats [by] May Eustace & Elizabeth Towe
	...
Cat breeds – Thailand
	Mǣo Thai / Sutthilak ʻAmphanwong
</pre>

The catalogers were quite unhappy with the system because it ignored a key aspect of the data that they were creating. The catalog users, however, loved it - because it provided keyword searching.

## Keyword Searching, or "Words out of Context"

Most of the content of the cataloging rules governs the creation of headings. These rules are quite complex but if followed turn out a consistent result. The problem is that the catalog users are not aware of those rules, and even if they were it takes years of experience to master them. In searching the card catalog, users had to try to find the right starting point for a left-to-right search. This is not only difficult, in some cases there is no way to discover all of the headings that might be of interest. For example, geographic locations can appear at the beginning, the middle or the end of a search, and may be given an inverted form in some cases:

<pre>
Boats and boating--Erie, Lake--Maps.
Books and reading--Lake Erie region.
Lake Erie, Battle of, 1813.
Erie, Lake--Navigation</pre>


