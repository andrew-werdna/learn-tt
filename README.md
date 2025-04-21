# learn-tt


Lots of people seem curious about type theory but it's not at all
clear how to go from no math background to understanding "Homotopical
Patch Theory" or whatever the latest cool paper is. In this repository
I've gathered links to some of the resources I've personally found
helpful.

## A Disclaimer

At this point `learn-tt` is a few years old and I can write with slightly more confidence than when
I first created this document. I still stand by the fact that the links in this list have helped me
learn ideas that would have been difficult to find elsewhere. At the same time, I worry that this
list carries more of a ring of authority than I wish it did, particularly now that it is relatively
popular. I learn more about type theory every day (admittedly, some days more slowly than I wish)
and my views on what constitutes a good explanation, a good approach, or even a good type theory
have changed in small and large ways since I first compiled these resources.

I toyed with the idea of deleting this repository because I have worried whether or not presenting
my own learning path does more harm than good. I have decided to leave it around but to add a
disclaimer instead.

> What follows below should not be construed as some _blessed path_ for learning type theory. You
> may find it better to skim this list or simply snort and ignore it entirely. My process for
> learning continues to be distinctly wandering and non-linear. Someone with different goals than me
> would find some of these links useless and I would not be nearly so bold as to claim that these
> resources are canonical, necessary, or even helpful for everyone. I can only hope that you enjoy
> reading them as much as I have.
>
> Daniel

### An addendum to this disclaimer

A few years after this disclaimer was written and roughly 10 years after making this repository, I
began writing my own introductory textbook on type theory together with [Carlo
Angiuli](https://carloangiuli.com).[^1] At the risk of singing our own praises, I think the current
draft is not terrible and it can be found freely available on [my
website](https://www.danielgratzer.com/papers/type-theory-book.pdf). Feedback on this draft is more
than welcome. Note that this book does not supplant most the resources listed below. However, it
hopefully it supplements a few of them.


[^1]: In a small twist of fate, Carlo is one of the authors of the "homotopical patch theory" paper
  referenced in the opening paragraph of this document. I didn't actually know Carlo well when
  making this document in 2015 and am honestly unsure what prompted me to choose that particular
  example.

## The Resources

### Textbooks

 - Practical Foundations of Programming Languages (PFPL)

    I reference this more than any other book. It's a very wide
    ranging survey of programming languages that assumes very little
    background knowledge. A lot people prefer the next book I mention
    but I think PFPL does a better job explaining the foundations it
    works from and then covers more topics I find interesting.

    * [Online copy (2nd Edition Preview)](https://web.archive.org/web/20230619030940/https://www.cs.cmu.edu/~rwh/pfpl/2nded.pdf)
    * [Dead-tree copy (2nd Edition)](https://www.amazon.com/Practical-Foundations-Programming-Languages-Robert/dp/1107150302)


 - Types and Programming Languages (TAPL)

    Another very widely used introductory book (the one I learned
    with). It's good to read in conjunction with PFPL as they
    emphasize things differently. Notably, this includes descriptions
    of type inference which PFPL lacks and TAPL lacks most of PFPL's
    descriptions of concurrency/interesting imperative languages. Like
    PFPL this is very accessible and well written.

   * [Online supplements](http://www.cis.upenn.edu/~bcpierce/tapl/)
   * [Dead-tree copy](https://mitpress.mit.edu/books/types-and-programming-languages)

 - Advanced Topics in Types and Programming Languages (ATTAPL)

   Don't feel the urge to read this all at once. It's a bunch of fully
   independent but excellent chapters on a bunch of different
   topics. Read what looks interesting, save what doesn't. It's good
   to have in case you ever need to learn more about one of the
   subjects in a pinch.

   * [Online supplements](http://www.cis.upenn.edu/~bcpierce/attapl/)
   * [Dead-tree copy](http://www.amazon.com/exec/obidos/ASIN/0262162288/benjamcpierce)

### Proof Assistants

One of the fun parts of taking in an interest in type theory is that
you get all sorts of fun new programming languages to play with. Some
major proof assistants are

 - Coq

    Coq is one of the more widely used proof assistants and has the
    best introductory material by far in my opinion.

    * [Official site](https://coq.inria.fr/)
    * [Software Foundations](http://www.cis.upenn.edu/~bcpierce/sf/current/index.html)
    * [Certified Programming with Dependent Types](http://adam.chlipala.net/cpdt/)
    * [The paper on the calculus of constructions](https://hal.inria.fr/inria-00076024/document)
    * [A paper on the calculus of inductive constructions](https://hal.inria.fr/hal-01094195/document) (What Coq
      is based on)
 - Lean

   Lean is one of the newer proof assistants on the scene. To be perfectly honest I haven't done a
   lot of proving in Lean yet but it seems neat. (If you have any resources you'd like to add to
   this list, please let me know)

   - [Official site](https://leanprover.github.io)
   - [Lean Manual](https://lean-lang.org/lean4/doc/)
   - [Functional Programming in Lean](https://lean-lang.org/functional_programming_in_lean/title.html)
   - [Logic and Proof Textbook](https://leanprover.github.io/logic_and_proof/)

 - Agda

    Agda is in many respects similar to Coq, but is a smaller language
    overall. It's relatively easy to learn Agda after Coq so I
    recommend doing that. Agda has some really interesting advanced
    constructs like induction-recursion.

    * [Official site](http://wiki.portal.chalmers.se/agda/pmwiki.php)
    * [Tutorial](http://www.cse.chalmers.se/~ulfn/papers/afp08/tutorial.pdf)
    * [Records tutorial](http://wiki.portal.chalmers.se/agda/pmwiki.php?n=ReferenceManual.RecordsTutorial)
    * [Conor McBride's](https://github.com/pigworker/MetaprogAgda) [fun Agda code](https://github.com/pigworker/CS410-14)
    * [Martín Hötzel Escardó's notes on Univalent Mathematics in Agda](https://www.cs.bham.ac.uk/~mhe/HoTT-UF-in-Agda-Lecture-Notes/HoTT-UF-Agda.html)

 - Idris

    It might not be fair to put Idris in a list of "proof assistants"
    since it really wants to be a proper programming language. It's
    one of the first serious attempts at writing a programming
    language with dependent types *for actual programming* though.

    * [Official site](http://idris-lang.org/)
    * [An actual introductory book](https://www.manning.com/books/type-driven-development-with-idris)
    * [Quick tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)
    * [A list of talks on Idris](https://www.youtube.com/watch?v=O1t4xJzrOng)
    * [David Christiansen's cool talk](https://www.youtube.com/watch?v=dP2imvL92sY)

 - Twelf

    Twelf is by far the simplest system in this list, it's the
    absolute minimum a language can have and still be dependently
    typed. All of this makes it easy to pick up, but there are very
    few users and not a lot of introductory material which makes it a
    bit harder to get started with. It does scale up to serious use
    though.

    * [Official site](http://twelf.org/)
    * [Wiki Tutorials](http://twelf.org/wiki/Tutorials)
    * [My tutorial](http://jozefg.bitbucket.io/posts/2015-02-28-twelf.html)
    * [The paper on LF, the underlying system of Twelf](http://citeseer.ist.psu.edu/viewdoc/summary?doi=10.1.1.21.5854)

### Type Theory

 - The Works of Per Martin-Löf

   Per Martin-Löf has contributed a *ton* to the current state of
   dependent type theory. So much so that it's impossible to escape
   his influence. His papers on Martin-Löf Type Theory (he called it
   Intuitionistic Type Theory) are seminal.

    If you're confused by the papers above read the book in the next
    entry and try again. The book doesn't give you as good a feel for
    the various flavors of MLTT (which spun off into different areas
    of research) but is easier to follow.

   * [1972](https://github.com/michaelt/martin-lof/blob/master/pdfs/An-Intuitionistic-Theory-of-Types-1972.pdf?raw=true)
   * [1979](https://github.com/michaelt/martin-lof/blob/master/pdfs/Constructive-mathematics-and-computer-programming-1982.pdf?raw=true)
   * [1984](https://github.com/michaelt/martin-lof/blob/master/pdfs/Bibliopolis-Book-retypeset-1984.pdf?raw=true)
   * [The Complete Works of Per Martin-Löf](https://github.com/michaelt/martin-lof)

 - Programming In Martin-Löf's Type Theory

   It's good to read the original papers and here things from the
   horses mouth, but Martin-Löf is much smarter than us and it's nice
   to read other people explanations of his material. A group of
   people at Chalmers have elaborated it into a book.

   * [Online link](http://www.cse.chalmers.se/research/group/logic/book/book.pdf)

 - The Works of John Reynolds

   John Reynolds' works are similarly impressive and always a pleasure
   to read.

   * [Types, Abstraction and Parametric Polymorphism](http://www.cse.chalmers.se/edu/year/2010/course/DAT140_Types/Reynolds_typesabpara.pdf) (Parametricity for
     System F)
   * [A Logic For Shared Mutable State](http://www.cs.cmu.edu/~jcr/seplogic.pdf)
   * [Course notes on separation logic](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/fox-19/member/jcr/www15818As2011/cs818A3-11.html)
   * [Course notes on denotational semantics](http://www.cs.cmu.edu/~jcr/cs819-00.html)

 - Homotopy Type Theory

   A new exciting branch of type theory. This exploits the connection
   between homotopy theory and type theory by treating types as
   spaces. It's the subject of a lot of active research but has some
   really nice introductory resources even now.

   * [The HoTT book](http://homotopytypetheory.org/book/)
   * [Student's Notes on HoTT](https://github.com/RobertHarper/hott-notes)
   * [Materials for the Schools and Workshops on UniMath](https://github.com/UniMath/Schools)

### Proof Theory

 - Frank Pfenning's Lecture Notes

    Over the years, Frank Pfenning has accumulated lecture notes that
    are nothing short of heroic. They're wonderful to read and almost
    as good as being in one of his lectures.

    * [Introductory Course](http://www.cs.cmu.edu/~fp/courses/15317-f09/)
    * [Linear Logic](http://www.cs.cmu.edu/~fp/courses/15816-s12/)
    * [Modal Logic](http://www.cs.cmu.edu/~fp/courses/15816-s10/)

 - Jean-Yves Girard's Books

   Girard, one of the most influential logicians of our time, has
   written several excellent texts on proof theory and logic. My
   ability to appreciate them is somewhat hampered by a language
   barrier but what work is available in English I have enjoyed.

   * [Proofs and Types](http://www.paultaylor.eu/stable/prot.pdf)
   * [The Blind Spot: Lectures on Logic](http://www.ems-ph.org/books/book.php?proj_nr=136&srch=browse_authors%7CGirard%2C+Jean-Yves)
   * [Mustard Watches: An Integrated Approach to Time and Food](http://girard.perso.math.cnrs.fr/mustard/page1.html)

### Category Theory

Learning category theory is necessary to understand some parts of type
theory. If you decide to study categorical semantics, realizability,
or domain theory eventually you'll have to buckledown and learn a
little at least. It's actually really cool math so no harm done!

 - Category Theory in Context

   A newly released textbook on category theory with a focus on using
   representable functors as a tool to place various concepts of
   category theory in a coherent framework. This has the substantial
   advantage of being freely available online! It's also published by
   Dover so the actual book itself is remarkably cheap.

   * [Online version](http://www.math.jhu.edu/~eriehl/context.pdf)
   * [Dead-tree version](http://store.doverpublications.com/048680903x.html)
   * [The author's post on the book](https://golem.ph.utexas.edu/category/2016/11/category_theory_in_context.html)

 - Practical Foundations of Mathematics

   This books does an excellent job of tying together general
   mathematics into the framework of category theory. It is
   accordingly covers a large basis of *math* outside of the field of
   category theory. It contains a large amount of categorical logic
   which warrants its inclusion in this list and is one of the more
   approachable texts on categorical logic. At least for me.

   * [HTML version](http://www.paultaylor.eu/~pt/prafm/)
   * [Dead-tree version](https://www.amazon.com/gp/product/0521631076)

 - Category Theory

   One of the better introductory books to category theory in my
   opinion. It's notable in assuming relatively little mathematical
   background and for covering quite a lot of ground in a
   readable way.

   * [Dead-tree version](http://www.amazon.com/Category-Theory-Oxford-Logic-Guides/dp/0199237182/ref=sr_1_1?ie=UTF8&qid=1439348930&sr=8-1&keywords=awodey+category+theory)

 - Ed Morehouse's Category Theory Lecture Notes

   Another valuable piece of reading are these lecture notes. They
   cover a lot of the same areas as "Category Theory" so they can help
   to reinforce what you learned there as well giving you some of
   the author's perspective on how to think about these things.

   * [Online copy](https://emorehouse.wescreates.wesleyan.edu/research/notes/intro_categorical_semantics.pdf)

 - Categorical Logic and Type Theory

   This book is honestly quite difficult to get through, but it's an
   absolutely indispensable resource for folks interested in
   categorical logic. More generally, this book contains one of the
   few coherent and comprehensive accounts of how to model type theory
   categorically. It is *not* a book to learn category theory or type
   theory from, it demands a good understanding of both since it's
   focused on applying category theory, not explaining it so
   much. This is also the book to read if you're interested in
   understanding the theory of fibered categories in general (the
   style of categorical semantics that it uses).

   * [Jacob's thesis, containing much of what went into the book](http://www.cs.ru.nl/B.Jacobs/PAPERS/PhD.ps)
   * [A definitely not suspicious online copy](https://people.mpi-sws.org/~dreyer/courses/catlogic/jacobs.pdf)
   * [Dead-tree copy](https://www.amazon.com/exec/obidos/ASIN/0444501703/qid%3D922441598/002-9790597-0750031)

 - Introduction to Higher-Order Categorical Logic

   This is a relatively short book on categorical logic that
   introduces all the basic concepts you needed to model simple
   higher-order logics in category theory. It is *much* easier reading
   than Categorical Logic and Type Theory but correspondingly less
   comprehensive. It focuses mainly on modeling the simply typed
   lambda calculus in cartesian closed categories and then on
   modeling a richer type theory internally to a topos. It provides a
   basic explanation of topos theory so it's intelligible having read
   an introductory category theory book.

   * [Dead-tree copy](https://www.amazon.com/Introduction-Higher-Order-Categorical-Cambridge-Mathematics/dp/0521356539/ref=pd_sim_14_5?_encoding=UTF8&psc=1&refRID=V4H286NSZWK4MWDPV17R)

 - Sheaves in Geometry and Logic

   This is not an ideal first book on category theory by any
   stretch. It merits inclusion because there are deep and interesting
   relationships between topos theory and type theory and this is one
   of the more approachable introductions. Some knowledge of topology
   would be helpful in understanding some of the examples in this
   books but I am told it is possible to muscle your way through
   without it.

   * [Dead-tree version](https://www.amazon.com/Sheaves-Geometry-Logic-Introduction-Universitext/dp/0387977104)

### Other Goodness

 - Gunter's "Semantics of Programming Language"

   While I'm not as big a fan of some of the earlier chapters, the
   math presented in this book is absolutely top-notch and gives a
   good understanding of how some cool fields (like domain theory)
   work.

   * [Dead-tree version](http://www.amazon.com/Semantics-Programming-Languages-Structures-Foundations/dp/0262071436/ref=sr_1_1?ie=UTF8&qid=1439349219&sr=8-1&keywords=gunter+semantics+of+programming+languages)

 - Abramsky and Jung's "Domain Theory"

   This what I reference nowadays for domain theory. It's a very good
   (if a little dense) introduction covering all the basic mathematics
   necessary to work with domains productively.  It should definitely
   be possible to follow if you've read some of Gunter's book.

   - [CiteSeerX link](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.50.8851)

 - Realizability: An Introduction to Its Categorical Side

   Categorical realizability is a fascinating area of overlap between
   type theory and category theory that, frustratingly, lacks many
   approachable introductions. van Oosten's book does a good job going
   through the basic aspects of categorical realizability. It is
   heavily dependent on knowledge of category theory though, I would
   recommend making it through Sheaves and Geometry and Logic (see
   above) or something equivalent first.

   * [Dead-tree version](https://www.amazon.com/Realizability-Introduction-its-Categorical-Side/dp/0444550208)

 - OPLSS

   The Oregon Programming Languages Summer School is a 2 week long
   bootcamp on PLs held annually at the university of Oregon. It's a
   wonderful event to attend but if you can't make it they record all
   their lectures anyways! They're taught be a variety of lecturers
   but they're all world class researchers.

   * [2012](https://www.cs.uoregon.edu/research/summerschool/summer12/curriculum.html)
   * [2013](https://www.cs.uoregon.edu/research/summerschool/summer13/curriculum.html)
   * [2014](https://www.cs.uoregon.edu/research/summerschool/summer14/curriculum.html)
   * [2015](https://www.cs.uoregon.edu/research/summerschool/summer15/curriculum.html)
   * [2016](https://www.cs.uoregon.edu/research/summerschool/summer16/curriculum.php)
   * [2017](https://www.cs.uoregon.edu/research/summerschool/summer17/topics.php)
   * [2018](https://www.cs.uoregon.edu/research/summerschool/summer18/topics.php)
