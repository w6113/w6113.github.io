---
layout: index
---


#### Overview


LLMs have opened new possibilities of automated agents that plan and complete tasks on the user’s behalf.  Such agents have the potential to usher in a new industrial revolution by automating organizational processes.   However, agents are currently limited to soft-edge tasks that have large tolerances for error, and are too unreliable for hard-edge tasks, like in healthcare or enterprises, where accuracy and reliability are paramount.  In short, what does it take for agents to be used in enterprises?

This graduate-level course will cut across the technology stack to examine the research questions that need to be answered for agents to be possible in real tasks that matter.    Each session will review 1-3 papers or systems, and discuss research opportunities that arise from the gap between existing research and enterprise requirements.  Topics will span systems (data systems and ML systems), AI (LLMs, agent-based planning), HCI, and theory (reinforcement learning, markets).   

Broad questions include

* What mechanisms are data systems missing to support agents?
* How does human-computer interaction change when the human interacts with agents?
* How can knowledge throughout an organization be used to constrain and improve agentic planning?
* How can systems handle the 10-100x increase in load generated by agents?
* What are the theoretical limits of what agents can do?
* At scale, how will the use of agents affect markets, incentives, and the structure of organizations?

Due to the speculative nature of the course, students are expected to co-investigate the problems alongside the instructors.   

Prereqs:

* Participants are expected to have exposure to LLM-agents, and expertise in another 
* This is by default a PhD-level course due to its research and forward looking nature
* This seminar is open to undergraduates and MS students with demonstrated abilities to critically read research papers and ask good questions.



#### Information 

* Class: Tu/Th 10:10-11:25AM, Loc TBA
* Instructors: 
  * [Eugene Wu](http://www.eugenewu.net)
  * [Kostis Kaffes](https://www.cs.columbia.edu/~kkaffes/index.html)
* [Syllabus & FAQ](./syllabus),
[Slack](https://w6113-s25.slack.com),
[Project](./projects), 
[Papers](./papers)
* Prereqs: W4111 Intro to DB (required), W4112 DB Implementations (recommended).  Ugrads OK; see Prof Wu

#### Grading 

* Discussion Prep 30%
* Class participation 30%
* [Project](./projects) 40%:
   Final Presentation <small>10%</small>,
   Paper <small>30%</small>

#### Recent Announcements


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
    <!--<th style="width: 15%;"> <p> <span>Assigned</span> </p> </th>
    <th style="width: 15%;"> <p> <span>Due</span> </p> </th>-->
  </tr>
  </thead>
{% assign idx = 0 %}

{% for r in site.data.schedule %}
  {% assign idx = idx | plus: 1  %}

  <tr style="background-color: {{r.color}}; ">
    <td class="date">C{{idx}}: {{r.date}}</td>
    <td class="slug">
      {% if r.link %}
        <a href="./papers#{{r.link}}"><b>{{r.slug}}</b></a>
      {% else %}
        <b>{{r.slug}}</b>
      {% endif %}

      {% if r.papers %}
      <ul>
      {% for p in r.papers %}
        <li><a href="{{p.url}}">{{p.title}}</a></li> 
      {% endfor %}
      </ul>
      {% endif %}

      {% if r.presenter %}
        <br/>
        <span class='presenter'>Presenter: {{r.presenter}}</span>
      {% endif %}

      {% if r.misc %}
      <div> {{r.misc|raw}}</div>
      {% endif %}

    </td>
    <td class="notes">
      {% if r.notes %}
        {{r.notes|raw}}
      {% endif %}
    </td>
    <!--
    <td>{{r.assigned | safe}}</td>
    <td>{{r.due | safe}}</td>
    -->
  </tr>
{% endfor %}

</table>


Course design inspired by

* [Cal's CS286](https://cs286berkeley.net/)
* [Waterloo's CS848](https://cs.uwaterloo.ca/~kmsalem/courses/cs848S19/schedule.shtml)
* Colin Raffel's [Role playing seminar](https://colinraffel.com/blog/role-playing-seminar.html)
* Carl Vondrick's self supervision graduate seminar