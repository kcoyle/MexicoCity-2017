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
Erie, Lake--Navigation

Cooking, French
France--Antiquities
Alps, French (France)
French--America--History
French American literature
</pre>

Names of people and organizations seem like they should be obvious but they also present difficulties, especially in their inverted form. Each of the  names below is correctly cataloged according to the rules, but knowing where to look requires one to know the person's culture and language:

<pre>
De la Cruz, Melissa
Cervantes Saavedra, Miguel de
Mao, Zedong, 1893-1976
Arnaldur Indridason
</pre>

Users were now able to type a few words into a query, such as "lake erie," and could discover library holdings that they never would have found in the card system. This was a huge gain, but it also was a loss; a loss of context and precision. This loss is especially dire in a large catalog where the overall number of retrieved items makes it impossible for the user to browse them all and make an intelligent assessment of which are relevant. Although some library catalogs provide an advanced search that searches in specific fields, such as personal name or title, users tend to prefer the default "single search box" which they have learned to rely on thanks to Internet search engines. Doing a search in a single search box for the word "Darwin" brings up such diverse titles as:

<pre>
Darwin
• Darwin; A Graphic Biography : the Really
Exciting and Dramatic Story of A Man Who
Mostly Stayed at Home and Wrote Some Books
• Darwin; Business Evolving in the Information Age
• Emma Darwin, A Century of Family Letters,
1792-1896
• Java Cookbook
• Canals and Rivers of Britain
• The Crimson Hair Murders
• Darwin's Radio
</pre>

Some of these are retrieved on author names, such as "Darwin L. Teihet" while others reflect other uses of the word. 

Keyword searching breaks the organization that should be created by the headings. The question is: how can we get that back? How can we give users both a simple search but also a rich and helpful retrieved set? 

In fact, that was one of the motivations behind FRBR.

## FRBR: What You Should Know

I've always had trouble understanding FRBR. There seem to be some internal contradictions that just block my thought processes when I try to imagine a FRBR world. It helps to look at the history of FRBR, and how it came into being. Here is a general timeline:

<pre>
Timeline
1990 – Stockholm meeting (IFLA)
1992 – Terms of reference completed
1994 – First draft for comment
1998 – Final draft
2009 – Current draft
2013 – RDA was implemented referencing FRBR
2016 – FRBR-Library Reference Model
2017 -Today
</pre>

The FRBR story began at an IFLA meeting in Stockholm in 1990, where representatives of national libraries had gathered to discuss the requirements for shared cataloging. The general agreement there was the current requirements for a national cataloging record were too expensive for the libraries to adhere to. They group decided on a project with the following goals:

1. Develop a framework for understanding bibliographic record
purposes
2. Recommend basic level of functionality for national library
bibliographic records
3. Develop core-level standard to reduce cataloging costs
4. Ensure that records meet user needs

From this it is clear why the effort was called "Functional Requirements for Bibliographic Records."

The study group was formed in 1992 with a document entitled "Terms of Reference". That document was developed by Tom Delsey of the National Library of Canada and Henriette Avram of the Library of Congress. The terms of reference gave the charge to the working group and defined its deliverables. Oddly, those deliverables differ considerably in their wording from the goals of the 1990 meeting.

Terms of Reference Deliverables

1. A framework with a range of entities and relationships
2. Define functions for entities
3. Identify attributes for entities
4. Define a national bibliographic record

Without stating it explicitly, the terms of reference given to the working group had the goal of solving the "relational database problem" of MARC - the fact that the MARC record was not designed in such a way that it could fit into the entity-relation model of relational database design. The terms used in the terms of reference came directly from the relational design work: "entities", "relationships" and "attributes." In fact the terms of reference cited a well-known 1984 book, '''Data Analysis; the Key to Database Design''', by Richard Perkinson, for the definition of the terms. The final report of the FRBR group affirmed this in its section on methodology:

  The methodology used in this study is based on an entity analysis technique that is used in the development of conceptual models for relational database systems.
  
Moving to an entity-relation model for bibliographic data was not in any way a bad idea, and had that model prevailed early in the 1990's decade we would mostly likely have a very different library systems environment than we have today. However, the FRBR final report, issued in 1998 and revised in 2009, still has not been reflected in library systems, and the era of relational databases is now firmly behind us. In addition, there is some confusion as to whether FRBR is intended as a step to a new data model, or whether it is an abstract expression of the bibliographic universe.

Two people who participated both in the FRBR study group and in the development of RDA express very different views. Barbara Tillett, in her 2005 Library of Congress publication on FRBR says:

  “FRBR is not a data model. FRBR is not a metadata
scheme. FRBR is not a system design structure. It is a
conceptual model of the bibliographic universe.” 

Tom Delsey, one of the co-authors of the terms of reference for FRBR and a member of both FRBR and the main editor of RDA, produced a document showing RDA's employment of FRBR concepts as an actual database design.

[page]

Within the FRBR document itself there are both statements that the model is conceptual as well as lists of entities and attributes and E-R diagrams that look very much like data models. Exactly what we should take away from FRBR and how it should influence the future of bibliographic data remains unclear. Yet FRBR does give us some positive steps toward a post-MARC future. The use of actual entities for persons and subjects can be used to create richer information about these entities than the identifying strings that we are limited to today. For example, a person entity can have biographical information as well as relationships with other entities. And FRBR introduces potentially actionable bibliographic relationships which can be much more helpful in a catalog than the mere informative notes that we mainly have today. Once we begin using these relationships in systems they may stimulate ideas for other relationships that could be added such as highlighting intellectual influence between works through citations and references.

What FRBR has not yet given us is an alternative to the string-based data that preponderates in library cataloging. It also has not resulted in a consensus for future catalog design. Both of these, however, are be studied in projects that are looking at the W3C's RDF model for library data.

Before moving on I should mention the lastest FRBR development, that of the FRBR Library Reference Model, or FRBR-LRM, and RDA. The FRBR-LRM is proposed as a consolidation of three "FR" models: FRBR, FRAD (authority data), and FRSAD (subject data). Unfortunately, the FRBR-LRM is even further from the library user's terminology, using latin terms '''res''' and '''nomen''' for '''thing''' and '''name'''. Also, the position of nomen in the model perpetuates the idea of strings as entities, something we should move away from as much as possible. RDA embodies the conceptual model of FRBR and will soon include some changes introduced in FRBR-LRM. We don't really know how the use of FRBR entities could or will change library cataloging, however, because RDA is currently being coded in MARC and therefore the entities are poorly represented, if at all. 

## Moving on to RDF

RDF is the W3C standard for web-based data that has a very simple underlying model of entities and relationships, although it differs  from the relational E-R model, for which it is considered a replacement. The entities and relationships provided by FRBR belong to that earlier model but provide a stepping stone to the RDF model. RDF could help us integrate library resources with other resources on the Web because it uses Web-based identifiers for all data. To take advantage of this, however, we have to embrace data that is not dependent on string-based identities, and this is a real change in how we create and store key bibliographic information.

BIBFRAME is a project initiated at the Library of Congress that uses RDF. It is also related to FRBR but does not entirely embrace the FRBR model. In fact, many of the entities that are defined in BIBFRAME are ones that could easily have been developed even if FRBR had not existed because they are the obvious contents of bibliographic data: resources, agents, topics. 

Unfortunately, the current emphasis in BIBFRAME development is in the translation of MARC records into BIBFRAME. This means that there is little innovation in the content of bibliographic records, so once again we are carrying forward the same data from older techbnology to a new technology and therefore not taking advantage of the promises that the newer technology offers. The phrase often used is "old wine in new bottles" but that actually sounds more positive than "old data in a new serialization." 

BIBFRAME also has not yet embraced interoperability with non-library resources. With RDF, interoperability is often achieved by re-using vocabularies that are shared by other communities. BIBFRAME's vocabulary is unqiue to BIBFRAME and therefore exists as a silo. There are ways to connect vocabularies for the sharing of data, and hopefully that is in BIBFRAME's future.

## The Future Catalog: Many Questions, Few Answers

There are some general areas that we need to think about when we address the future of library catalogs. These are some of them, but surely not all.

### It's all technology (except the users)

Every generation of library catalogs has been a technology, from those clay tablets to book catalogs to cards and now the computer. Both FRBR and RDA make statements that they are "technology neutral" - but they are not. FRBR made use of the concepts of database management technology of the 1980's and 1990's and that influenced its design. RDA continues to describe the creation of left-anchored strings that made up the structure of the card catalog. Unless modelers are aware of the technology behind their designs, and the assumptions they are using for development, they risk being technology ignorant. 

The aspect of deisgn that is not technology is the human users. These users and their needs should be the primary focus of any standards. FRBR claimed to be built around user needs in the form of the user tasks that it defined. Those user tasks were not well-defined, however. Out of the 142 pages of the FRBR final report, one half of one page was dedicated to defining the user tasks "find, identify, select, and obtain." Although numerous pages of tables that matched user tasks to attributes, nowhere did the report state '''how''' the attributes fulfilled those tasks. 

FRBR "find" is particularly insufficient to guide any type of metadata or systems development. The FRBR final report defines "find" as:

  "to find entities that correspond to the user’s stated search criteria (i.e., to locate either a single entity or a set of entities in a file or database as the result of a search using an attribute or relationship of the entity);"
  
The FRBR-LRM gives this definition:

  "To bring together
information about
one or more
resources of
interest by
searching on any
relevant criteria"

As a starting point either of these defintions might be acceptable, but there is so much more that needs to be said before any intelligent modeling can take place that would support this activity. What will be the basis of searching? What will determine result sets? Will there be one or more ordering of results? What options will be presented for exploration within the bibliographic universe?

Another key question is whether the library's responsibility truly ends at "obtain." Locating and obtaining a document or resource is only the beginning of the purpose of providing those resources to begin with. Some years ago a grant project looked at the uses of resources among faculty members. The results were broken into four activity types: discover, gather, share, and create. Of these, only a small portion of the sub-activities under "discover" are covered by the FRBR user tasks. Others are important tasks such as keeping current in one's field, sharing discovery with collaborators, and using the results of recommender systems. Not all of the tasks in the study might directly involve the library, but clearly good library service will support as many information tasks as possible. 

[diagram & citation]


