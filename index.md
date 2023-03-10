---
layout: index
---


#### Overview

Data management systems are the corner-stone of modern applications, businesses, and science (including data).  If you were excited by the topics in 4111,  this graduate level course in database systems research will be a deep dive into classic and modern database systems research.  Topics will range from classic database system design, modern optimizations in single-machine and multi-machine settings, data cleaning and quality, and application-oriented databases.

The class places a heavy emphasis on paper reading and writing good paper reviews. The point is to practice reading papers critically, writing proper reviews, implementing ideas in research papers, and conducting research. As such, students will be expected to read papers in depth, complete assignments based ideas from the readings, and conduct a semester-long research project.

Ideally, you will be comfortable with reading code that is not yours, open to trying different software systems, and willing to actively participate in and lead discussions.

See [FAQ](./syllabus#faq) for difference between 6113 and the other database courses. 

<small style="color: grey">Course capped at 25. </small>



#### Recent Announcements
* (12/10) Deadline for report submission is extended by 1 day to Tue, December 15, 2020 11:59PM
* (11/2) A3 solution is and assignment A4 is released.
* (10/30) PC Reviews are out. The first review will be due 11/06 10AM (due to election) while the second review will be due at the normal time 11/09 10AM
* (10/22) The regular class on next Tuesday 10/27 will be replaced with a Guest Lecture about Streaming DB by Prof. Vasiliki at 4-5:30PM EST. Zoom link for the lecture is shared on slack and will be recorded. Paper reviews proceed as usual.


#### Tentative Schedule


<style>
.presenter { }
</style>

<table class="table table-striped schedule">
  <thead>
  <tr>
    <!--<th class="idx" style="width: 3em; max-width:3em;"></th>-->
    <th class="date" style="width: 15em; max-width: 15em;"> <p> <span>Date </span> </p> </th>
    <th style="min-width: 15%;"> <p> <span>Topic </span> </p> </th>
    <th style="width: 10%"> <p> <span>Notes </span> </p> </th>
    <th style="width: 15%;"> <p> <span>Assigned</span> </p> </th>
    <th style="width: 15%;"> <p> <span>Due</span> </p> </th>
  </tr>
  </thead>
{% assign idx = 0 %}

{% for r in site.data.schedule %}
  {% assign idx = idx | plus: 1  %}
  <tr style="background-color: {{r.color}}; ">
    <!--<td class="idx">C{{idx}}</td>-->
    <td class="date">C{{idx}}: {{r.date}}</td>
    <td class="slug">
      {% if r.link %}
        <a href="./papers#{{r.link}}"><b>{{r.slug}}</b></a>
      {% else %}
        <b>{{r.slug}}</b>
      {% endif %}
      {% if r.presenter %}
        <br/>
        <span class='presenter'>Presenter: {{r.presenter}}</span>
      {% endif %}
      {% if r.notes %}
        <br/>
        {{r.notes|raw}}
      {% endif %}
      </td>
    <td class="notes">
    </td>
    <td>{{r.assigned | safe}}</td>
    <td>{{r.due | safe}}</td>
  </tr>
{% endfor %}
</table>



<!--
#### Tentative list of papers for last lectures

* Approx Query Processing
  1. Sampling basics and challenges
  2. CONTROL, Blink, Sample-and-seek, AQP++
* Streaming
  1. Windowed Streaming
    * DataFlow paper
    * CQL/Stream project
    * TelegraphCQ
  2. Complex event processing
    * SASE
* X in DBs
  * ML in SQL
    * MADLib
    * SystemML
    * Learning over joins
  * Graph in SQL
    * Jignesh's papers
    * Vertexica
    * RecStep
  * Vis in SQL
-->


<!--

Topics will cover a subset of papers from [the redbook](http://www.redbook.io), as well as modern provenance/lineage, data analysis, cleaning, and perhaps databases+ML.


* Intro
  1. Syllabus + life of a query + meta stuff
    * Codd
  2. DB primer/background
    * Storage hierarchies and [numbers you should know](https://gist.github.com/hellerbarde/2843375)
    * The importance of simple equations
    * 5 minute rule
    * Other principles
* Basics
  1. [Architecture of a DB](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)
  2. [SystemR retrospective](http://db.cs.berkeley.edu/cs262/SystemR-annotated.pdf) or   
     [Design of Postgres](http://db.cs.berkeley.edu/cs286/papers/postgres-cacm1986.pdf)
* Indexes
  1. R-trees
  2. [GIST-trees](http://db.cs.berkeley.edu/papers/vldb95-gist.pdf)
* Joins
  1. Shapiro: Join Processing in Database Systems with Large Main Memories  
  2. Track Join (Wangda?)
* Execution
  1. Volcano's Exchange
    * https://people.eecs.berkeley.edu/~brewer/cs262/exchange+eddies.html
  2. Eddies
* Lower level Optimizations
  * DBMin
  * [Hybrid Caching](http://db.cs.berkeley.edu/cs286/papers/caching-sigmod1996.pdf)
* Query Plan Optimization
  * Classics
    * Selinger
    * Cascades
    * Volcano Optimizer
  * Modern stuff
    * Using RL for join optimization
* Languages
  1. datalog
  2. schemaSQL
* Systems Architectures
  1. C-Store
    * Column-Stores vs. Row-Stores: How Different Are They Really?
  2. H-store/Hekaton
* Systems Architectures
  1. Query Compilation
    * T. Neumann, Efficiently Compiling Efficient Query Plans for Modern Hardware
    * K. Krikellas, et al., Generating Code for Holistic Query Evaluation, in ICDE, 2010
    * How to Architect a Query Compiler, Revisited
  2. ??
* Materialization for physical database design
  1. Materialized Views
    * Updating Materialized Views
    * Surajit's paper
      * http://www.vldb.org/conf/2007/papers/special/p3-chaudhuri.pdf
  2. Datacubes
    * Jim Gray paper
    * [Implementing data cubes efficiently](http://db.cs.berkeley.edu/cs286/papers/datacube-sigmod1996.pdf)
* Approx Query Processing
  1. Sampling basics and challenges
  2. CONTROL, Blink, Sample-and-seek, AQP++
* Streaming
  1. Windowed Streaming
    * DataFlow paper
    * CQL/Stream project
    * TelegraphCQ
  2. Complex event processing
    * SASE
* X in DBs
  * ML in SQL
    * MADLib
    * SystemML
  * Graph in SQL
    * Jignesh's papers
    * Vertexica
* X in DBs
  1. Vis in SQL

-->
<!--

* Distributed Query Processing
  1. Gamma: distributed Joins
  2. 
* Concurrency Control
  1. Serializability, Linearizability, tec overview
  2. MVCC and OCC
* Basics of Plan Execution / optimization
  * SEDA?
  * dbmin
* Languages
  * SchemaSQL
  * datalog
* Storage
* Recovery
  * ARIES
  * H-store
* Architectures
  * C-Store + ten years later
  * Hekaton
  * MR/Spark
  * Naiad
  * Query compilation + Tarik
* Concurrency Control
  * MVCC vs OCC vs Pessimistic vs CALM
* Slightly modern stuff
  * In network execution?
  * ML in SQL
    * MADLib
    * SystemML
  * Graph in SQL
    * Jignesh's papers
    * Vertexica
* Scheduling
* Networking
-->
