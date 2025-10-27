---
content_type: page
description: This section provides the the schedule of weekly readings and a list
  of recommended books.
draft: false
learning_resource_types:
- Readings
ocw_type: CourseSection
title: Readings
uid: 6b6aaff6-5564-7548-6cac-616cb72ef1ea
---
The readings, in the form of short articles and papers, assigned for each class are listed in the table below. While there is no required textbook for the course, recommended books include:

Crockford, Douglas. *JavaScript: The Good Parts*. O'Reilly Media, 2008. ISBN: 9780596517748. \[Preview with {{% resource_link "e089289c-7727-4063-9164-7b44eae3b594" "Google Books" %}}\]

Fernandez, Obie. *The Rails 3 Way*. 2nd ed. Addison-Wesley Professional, 2010. ISBN: 9780321601667. \[Preview with {{% resource_link "fbf9b9d2-ad33-4839-9c18-ace6f7d2ed07" "Google Books" %}}\]

Fulton, Hal. *The Ruby Way, Second Edition*. 2nd ed. Addison-Wesley Professional, 2006. ISBN: 9780672328848.

Stefanov, Stoyan. *JavaScript Patterns*. O'Reilly Media, 2010. ISBN: 9780596806750. \[Preview with {{% resource_link "12129c05-8d1d-4d55-a2d0-f4f3cd61de6d" "Google Books" %}}\]

{{< tableopen >}}{{< theadopen >}}{{< tropen >}}{{< thopen >}}
WEEK #
{{< thclose >}}{{< thopen >}}
READING TOPICS
{{< thclose >}}{{< thopen >}}
READINGS
{{< thclose >}}{{< trclose >}}{{< theadclose >}}{{< tbodyopen >}}{{< tropen >}}{{< tdopen >}}
1
{{< tdclose >}}{{< tdopen >}}
**Introduction & Web Basics**
{{< tdclose >}}{{< tdopen >}}
No readings assigned
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
2
{{< tdclose >}}{{< tdopen >}}

**Routing & Model-View-Controller Design**

These readings introduce one of the most important concepts in software engineering: decomposing a problem into separate "concerns" and tackling them one-by-one. We will begin with Dijkstra's classic paper, in which he coined the term "Separation of Concerns." The exerpts from Fowler's book describe how this concept plays a critical role in development of modern software systems. In particular, you will read about a well-known design pattern called Model-View-Controller (MVC). While reading, think about how MVC is being used to structure popular web applications, such as Twitter and Amazon.

{{< tdclose >}}{{< tdopen >}}

Dikstra, E. W. "{{% resource_link "0ea15da9-7994-4cdd-a322-0909daedbfdc" "On the Role of Scientific Thought" %}}." In *Selected Writings on Computing: A Personal Perspective*. Springer, 1982, pp. 60–6. ISBN: 9780387906522.

Fowler, Martin. "The Three Principal Layers." Chapter 1 in *Patterns of Enterprise Application Architecture*. Addison-Wesley Professional, 2002. ISBN: 9780321127426. \[Preview with {{% resource_link "d25215e3-58fd-4bc6-a505-59edfd5d5090" "Google Books" %}}\]

———. "Model View Controller." Chapter 14 in *Patterns of Enterprise Application Architecture*. Addison-Wesley Professional, 2002. ISBN: 9780321127426.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Dependency & REST**

Dependency is one of the most important criteria for assessing the quality of software design. Tight, unnecessary coupling between different modules is a bad sign that often results in a gigantic implementation mess as the system evolves over time. In the first of the readings, you will be introduced to Parnas' seminal paper, where he discusses the "uses" relation as a technique for describing and reasoning about the dependency structure of software.

In the second part, you will read about REST, a style of designing web applications proposed by Roy Fielding (also one of the original designers of HTTP and Apache Server). Focus on high-level concepts that distinguish REST from other styles of web application design, and do not worry too much about Rails-specific details. (The book was published in 2008, and Rails has evolved significantly over the years.)

{{< tdclose >}}{{< tdopen >}}

Parnas, David L. "{{% resource_link "e3d567ea-f647-42bc-a50f-c907d53be20b" "Designing Software for Ease of Extension and Contraction" %}}." *IEEE Transactions on Software Engineering* 5, no. 2 (1979): 128–38.

Benson, Edward. "Resources and REST." Chapter 6 in *Art of Rails (Programmer to Programmer)*. Wrox, 2008. ISBN: 9780470189481. \[Preview with {{% resource_link "3bcfc5fc-208b-4d55-912a-7fbbec3695ce" "Google Books" %}}\]

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
3
{{< tdclose >}}{{< tdopen >}}

**Introduction to Data & Object Modeling**

When you begin designing your new application, you will have some mental model of different types of objects that exist in your system, and relationships between them. Writing down that model explicitly on a piece of paper is a really helpful exercise because it forces you to be clear about what that model actually is, and discover both silly and subtle mistakes that are harder to fix once the code is written. Trust us — do this early in the design of your app, and it will save you lots of time and effort later on!

In the reading, you will be introduced to two different notations that are intended to help you write these models down in a systematic way. You will read Chen's classic paper, which introduced the idea of entity-relationship (ER) models. The ER model has had a tremendous influence on many fields of computer science, especially on database design, and is still widely taught and used today. Again, focus on the high-level ideas, especially in the first three sections of the paper.

{{< tdclose >}}{{< tdopen >}}
Chen, Peter. "{{% resource_link "cbcd661a-deb7-45f9-b5a7-c4b8ea0b9204" "The Entity-Relationship Model – Toward a Unified view of Data" %}}." *ACM Transactions on Database Systems* 1, no. 1 (1976): 9–36.
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Relational Data Model**

In the last lecture, we discussed ER and object models as notations for building a conceptual model of relationships between different types of data objects. Eventually, for your app, you will need to take this model and encode it as concrete data inside a database. Many of today's databases systems are based on the idea of the relational data model, a way of organizing data in terms of relations. We will talk about how we can systematically transform an object model into a relational data model, as a first step in the design of your database. You will read a short article that introduces the basic elements of a relational data model: relations, attributes, and tuples, among others.

{{< tdclose >}}{{< tdopen >}}
Ullman, Jeffrey D., and Jennifer Widom. "The Relational Data Model." Chapter 3 in *A First Course in Database Systems*. Prentice-Hall, 1997, pp. 85–90. ISBN: 9780138613372. \[Preview with {{% resource_link "81075b0b-044e-44eb-9b41-e011ab478fa0" "Google Books" %}}\]
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
4
{{< tdclose >}}{{< tdopen >}}

**Design Concepts**

What makes a good software design? Software engineering is a relatively young field, and there's still a lot of on-going work (in both academia and industry) on developing principles and methods behind the design of successful software systems. In the readings, you will be introduced to some of the basic concepts that are considered an essential part of any good software design.

"Brilliance" is a short but illuminating piece about a property of design whose importance is often overlooked, especially in software development — namely, simplicity.

Nothing occurs in a vacuum; every program or system that you build will be part of some environment. You can't design a functional and reliable system without thinking about the context in which it operates. You will read a short snippet from Alexander's book, in which he describes design as the activity of finding a good fit between a "form" and its "context".

{{< tdclose >}}{{< tdopen >}}

Jackson, Michael A. "Brilliance." In *Software Requirements and Specifications: A Lexicon of Practice, Principles and Prejudices*. Addison-Wesley Professional, 1995, p. 20. ISBN: 9780201877120.

Alexander, Christopher. "Goodness of Fit." *Notes on the Synthesis of Form*. Harvard University Press, 1964, pp. 15–9. IBSN: 9780674627512. \[Preview with {{% resource_link "7db93d3d-61ec-42fa-9ca2-4418f7bb5d86" "Google Books" %}}\]

\*Read up to the first paragraph on page 19.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Conceptual Integrity**

In the last lecture, we looked at some basic design concepts that you should keep in mind while building your own applications. Continuing on the same thread, you will read a chapter from Brook's seminal book, The Mythical Man-Month, in which he introduces the idea of "conceptual integrity" as the key quality of software design.

{{< tdclose >}}{{< tdopen >}}
Brooks, Frederick P., Jr. "Aristocracy, Democracy, and System Design." Chapter 4 in *The Mythical Man-Month*. Addison-Wesley, 1975. ISBN: 9780201006506.
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
5
{{< tdclose >}}{{< tdopen >}}

**Programming Language Design**

Tony Hoare is an influential British computer scientist, perhaps best known for his invention of Quicksort. But he also made a number of long-lasting contributions to programming languages, software verification, and operating systems, for which he was awarded the Turing Award in 1980. The following lecture, which he gave during his acceptance of the award, contains many important lessons in programming language design that still remain relevant today (and sadly neglected by many designers).

{{< tdclose >}}{{< tdopen >}}
Hoare, C. A. R. {{% resource_link "86d1617b-db5d-4d0e-8722-0cacb5fd7e0e" "\"The Emperor's Old Clothes.\" (PDF)" %}} *Communications of the ACM* 24, no. 2 (1981): 75–83.
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Prototype-Based Programming**

SELF is an influential language that inspired, among others, Javascript and its variants. Unlike Java or other class-based languages, SELF is based on the concept of *prototypes*, which involves making *clones* of objects instead of instantiating them. You will read an introductory paper on SELF by the designers of the language. Think about how SELF differs from Java or other languages that you are already familiar with, and some trade-offs between prototypes vs. class-based approach to programming.

{{< tdclose >}}{{< tdopen >}}

Ungar, David, and Randall Smith. "{{% resource_link "1b3960fb-273d-4f67-9591-ee9626f6cc34" "SELF: The Power of Simplicity" %}}." *LISP and Symbolic Computation* 4, no. 3 (1991): 187–205.

\*You do not need to read Sections 4, 7, and 8.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}
6
{{< tdclose >}}{{< tdopen >}}

**Client-Side Programming**

Back in the old days of the Internet, most web applications were built on synchronous communication between a server and its clients. Whenever a client had a request to be fulfilled, it would wait for the server to process the request and return the response in form of an HTML page. As you can imagine, this resulted in a rather limited user experience; every time you edited a form or clicked on a link, you would have to wait until the browser loaded a new HTML page. But everything changed with Javascript and AJAX. The first of the readings is the article that introduced the term "AJAX," written by Garrett.

One thing you should always keep in mind while working on your next web app: It's a piece of software that will be viewed and used by *other* human beings. Sounds obvious, right? Surprisingly, there are a lot of apps out there where it's clear that the designer didn't think too hard about how the user would interact with the site. Porter's article introduces some basic principles that you should aim for when designing client-side interactions.

{{< tdclose >}}{{< tdopen >}}

Garrett, Jesse James. "Ajax: A New Appproach to Web Applications." *Adaptive Path*, February 18, 2005.

Porter, Joshua. "{{% resource_link "0b441fa1-2605-4b52-8bee-2fff332980cc" "Principles of User Interface Design" %}}." *Bokardo*.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
7
{{< tdclose >}}{{< tdopen >}}

**Structured Programming**

Tools such as Javascript, jQuery, and AJAX give you a lot of flexibility and power for building different types of client-side interactions. However, they could also make your code much more complex and harder to understand, so you should pay extra attention to the code design when using these tools.

GOTO is a seemingly innocuous instruction for jumping from one place to another in code. Back in the early days of computing, GOTO was a language feature regularly used by programmers, until Dijkstra pointed out the danger of overusing GOTO in his classic paper.

The points that he makes here seem rather obvious now, but back then, the paper caused a lot of controversy, and many people were strongly against the ideas in it (one reviewer of the paper went as far as saying "I am confident that, 30 years from now, the goto will still be alive and well and used as widely as it is today.").

A modern incarnation of the problem that Dijkstra describes is sometimes called *callback hell*. Unless you are judicious about the use of callbacks, you could easily end up with a mess of Javascript code that's difficult to understand and debug. Unfortunately, we don't yet have a proven alternative that we can use to implement complex client-side interactions. Thankfully, not all is lost: *Functional reactive programming (FRP)* is a style of programming that has recently surfaced as a potential solution to the callback hell. The following article, written by the designer of a FRP language called *Elm*, introduces the problem with callbacks and describes how FRP might be used to fix it. Focus on the high-level ideas behind FRP; you do not need to understand the details of the Elm language.

{{< tdclose >}}{{< tdopen >}}

Dijkstra, Edsger W. "Go To Statement Considered Harmful." *Communications of the ACM* 11, no. 3 (1968): 147–48.

Czaplicki, Evan. "{{% resource_link "6f66ad3f-e98e-49f1-9110-0149f2fc39fe" "Escape from Callback Hell" %}}." *Elm*.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Web Security**

Nowadays, almost every week, there's some news article about an exploit on a large corporation that ends up losing data for millions of customers, a denial-of-service attack that takes down a government web site, or a new security vulnerability in a popular application that must've been patched a thousand times by now. Security has been an active area of research in computer science for many decades, but it doesn't seem like things are getting much better every day. So why is it so hard to keep our computers secure?

In Zalewski's article, we will explore some of the reasons why the widespread use of the Internet makes security harder than it has ever been.

It turns out that there are a number of things that we could do to make our systems reasonably secure against common security attacks. Unfortunately, unlike in many other engineering fields, such as civil or aerospace, software engineers often neglect to learn from our past mistakes, leaving glaring holes in software that we already know how to fix. Ranum's article describes some of the most common security mistakes that we tend to repeat again and again.

{{< tdclose >}}{{< tdopen >}}

Zalewski, Michal. "Security in the World of Web Applications." Chapter 1 in *Tangled Web: A Guide to Securing Modern Web Applications*. No Starch Press, 2011, pp. 14–8. ISBN: 9781593273880. \[Preview with {{% resource_link "a2f7c5f9-1787-4466-abf9-7cc4b02e4045" "Google Books" %}}\]

Ranum, Marcus. {{% resource_link "fa34251a-c97a-4d5a-9cc7-42c2c8ada650" "\"Six dumbest Ideas in Computer Security.\" (PDF)" %}} *Ranum,* September 1, 2005.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}
8
{{< tdclose >}}{{< tdopen >}}

**Software Development Methods**

We will discuss different approaches to software development that have risen and faded in popularity over the last several decades. Advocates of current approaches (such as "agile") often imply that these approaches are radical departures from the past, but in fact their roots go back a long way.

Edsger Dijkstra was a strong advocate of a style of software development in which mathematical reasoning played a central role. His writings are well known for their uncompromising positions on many topics, even the most extreme of which usually contained profound insights.

(Unfortunately, this particular article uses a racist idiom; in 1978, at the time of writing, there was less of a consensus that offensive references of this sort should not be used.)

Brook's famous book, *The Mythical Man-Month*, is full of gems that have had long-lasting impact on the field of software engineering since its publication in 1975. One of them hinted at a style of development that was ignored for many years, but has become very popular in the last decade or so — namely, agile development. In the chapter from his book, you will read about the idea of building a system to eventually throw away, which may seem counter-intuitive at first.

{{< tdclose >}}{{< tdopen >}}

Dijkstra, Edsger. "{{% resource_link "51acb665-22d0-4e78-bf22-9ed2173837c5" "The pragmatic engineer versus the scientific designer" %}}." 1978.

Brooks, Frederick P., Jr. "Plan to Throw One Away." Chapter 18 in *The Mythical Man-Month: Essays on Software Engineering*. Addison-Wesley, 1975. ISBN: 9780201006506.

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen rowspan="2" >}}
9
{{< tdclose >}}{{< tdopen >}}

**Designing Dependable Software**

Computer programs are closer to human beings than some may believe. Not only do they run your favorite apps on your laptop and cellphone, but they are also used to control your car, house, electricity, heart monitor, and nearly every other critical aspect of your life. But it turns out that we know surprisingly little about how to design programs to be safe and reliable.

One of the most alarming examples of badly written software causing direct harm to people is in medical devices. Thimbleby's article describes some disturbing cases of catastrophic medical device failures due to bad interface design, and argues that we, as programmers, are responsible for designing a program to minimize the likelihood of such a failure.

You will also watch a related clip, which illustrates some of the points from the article.

{{< tdclose >}}{{< tdopen >}}

Thimbleby, Harold. "{{% resource_link "105b16c0-c627-400e-ba36-2a3d99817c58" "Ignorance of Interaction Programming is Killing People" %}}." *Interactions* 15, no. 5 (2008): 52–7.

———. "Saving Lives by Design." September 1, 2011. Youtube. {{% resource_link "215efd14-a146-4939-a5be-e3d84466bb2f" "www.youtube.com/watch?v=glwtlH0oYc0" %}}

{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}

**Presenting Your Ideas**

Having a good idea is just the beginning; you need to be able to communicate your ideas effectively to other people. For the upcoming final project in this class, your team will present your idea to the entire class and convince them that your app is the coolest thing that will ever be built.

But what distinguishes a great talk from a boring, seemingly mindless presentation? There is lots of advice out there on making a good presentation, but many agree that you need to be able to present a compelling story to engage your audience.

{{< tdclose >}}{{< tdopen >}}
Duarte, Nancy. *Resonate: Present Visual Stories that Transform Audiences*. Wiley, 2010, pp. 110–15. ISBN: 9780470632017.
{{< tdclose >}}{{< trclose >}}{{< tbodyclose >}}{{< tableclose >}}