---
layout: index
---

<!--<div class="alert alert-success" role="alert">
  <h4 class="alert-heading">Registering for this course</h4>
  <p>If you are interested in taking this course, please fill out 
  <a href="https://forms.gle/Z9RufMdoA1YSfa5HA" style="color:#045321; text-decoration:underline;"><b>THIS SHORT FORM</b></a>.
  Due to the small class size, we will use the answers to balance student backgrounds and expertise.  To ensure commitment, we are not currently accepting audits.  
  </p>
</div>
-->



# Overview


LLMs have opened new possibilities of automated agents that plan and complete tasks on the user’s behalf.  Such agents have the potential to usher in a new industrial revolution by automating organizational processes.   However, agents are currently limited to soft-edge tasks that have large tolerances for error, and are too unreliable for hard-edge tasks, like in healthcare or enterprises, where accuracy and reliability are paramount.  In short, what does it take for agents to be used in enterprises?

This graduate-level course will cut across the technology stack to examine the research questions that need to be answered for agents to be possible in real tasks that matter.    Each session will review 1-3 papers or systems, and discuss research opportunities that arise from the gap between existing research and enterprise requirements.  Topics will span systems (data systems and ML systems), AI (LLMs, agent-based planning), HCI, and theory (reinforcement learning, markets).   

Broad questions include

* What mechanisms are data systems missing to support agents?
* How does human-computer interaction change when the human interacts with agents?
* How can knowledge throughout an organization be used to constrain and improve agentic planning?
* How can systems handle the 10-100x increase in load generated by agents?
* What are the theoretical limits of what agents can do?
* At scale, how will the use of agents affect markets, incentives, and the structure of organizations?



### Class Structure

* There will be assigned readings for each week
* Classes will be a mix of discussion about the papers, speculating about new problems, and external speakers
* Due to the speculative nature of the course, students are expected to co-investigate the problems alongside the instructors.   

# Project ideas

**For 6113 Students Only**: [Google doc with suggestions](https://docs.google.com/document/d/19H-ZQ2ARwy-gUhOoUb9MqyWBNuVzCRTBlsNxAywlChQ/edit).  You are welcome to add your own ideas!



# Tentative Schedule



<span class="date">1/21</span>	<span class="topic">Introduction & a quick history of agents</span>	- Eugene & Kostis



<span class="date">1/23</span>	<span class="topic"><a href="https://drive.google.com/file/d/1308CxPBdqhrurz4zeGN5Uw_Xp6BzQaJ1/view?usp=sharing">Tutorial: Agents Overview</a></span> - [Xiao Yu](https://jasonyux.com/), Columbia {% include toggle.html content="I am a second year Ph.D. student in Computer Science at Columbia University advised by Zhou Yu. Before joining the Ph.D. program, I was an undergrad also at Columbia University, majoring in Computer Science and minoring in Applied Physics. Currently I am interested in: 1) Reinforcement Learning + (V)LM Training, and 2) Planning Algorithms + (V)LM Agents. My recent works include developing search algorithms to improve (V)LM's performance on dialogue tasks such as persuasion and agentic tasks such as using a web browser or a virtual machine; and methods to train (V)LMs without extensive human labeling efforts." %}

* Readings
    * [OSWorld](https://arxiv.org/abs/2404.07972)
    * [SWE-agent](https://arxiv.org/abs/2405.15793)
* Questions
    * What are some real life applications that can make use of/benefit from these computer agents? 
    * What are some concerns/limitations?


<span class="date">1/28</span>	<span class="topic"><a href="https://drive.google.com/file/d/1TUZf2GV3zPZA8sLKSSpkp2nd5OT8SSpt/view?usp=sharing">Tutorial: Agent Planning</a></span> - [Xiao Yu](https://jasonyux.com/), Columbia

* Readings
    * [AlphaGo](https://www.nature.com/articles/nature24270)
    * [Reflective-MCTS](https://arxiv.org/abs/2410.02052)
* Questions
    * What other tasks/domains would benefit from these self-learning/planning approaches? 
    * What key limitations or errors should you watch for when using these approaches?



<span class="date">01/30</span> <span class="topic">Background: SWEBench</span> - [John Yang](https://john-b-yang.github.io/), Stanford {% include toggle.html content="John Yang is a PhD student at Stanford University advised by Prof. Diyi Yang and Ludwig Schmidt. He formerly conducted research at Princeton University advised Prof. Karthik Narasimhan. John works on evaluations, data, and systems around Language Model (LM) agents for software engineering" %}

* Readings
  * [SWE-bench: Can Language Models Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770)
  * [SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering](https://arxiv.org/abs/2405.15793)
* Questions
  * What might the future of evaluations for Language Models and AI Systems look like? Can you think of any real world workflows or pipelines (not necessarily within Software Engineering or Tech) that might be interesting testbeds?
  * How might AI agents be deployed in a real world? How might the responsibilities of a software developer / manager and the technology market itself evolve in response to AI co-pilots?


<span class="date">02/04</span> <span class="topic">Programming Foundation Models</span> [Thomas Joshi](), Columbia {% include toggle.html content="Thomas Joshi is co-author of Stanford DSPy and leads the GenAI Collective, the largest AI community in the US with over 30,000 members across chapters in SF, NYC, Boston, London, Paris, and other cities. DSPy has been used by Nvidia, Microsoft, Meta, NASDAQ, Carlyle, ABN Amro, JetBlue, Cohere, and others. Thomas is passionate about modular approaches to AI system design, enabling engineers to optimize LLM pipelines for performance and cost-efficiency." %}

* Readings
  * [DSPy](https://arxiv.org/abs/2310.03714)
* Questions (rather than answering these, use the questions as a starting point for discussion on slack)
  * Modular frameworks like DSPy enhance flexibility and scalability in agentic systems but may introduce inefficiencies due to communication overhead between modules. How do these trade-offs affect the performance of agents in real-world applications? What strategies could be used to minimize these inefficiencies while retaining the advantages of modularity?
  * DSPy’s modular agents use predefined components tailored to specific tasks, but dynamic environments often demand adaptability. How can agents built with modular frameworks autonomously adapt or reconfigure their modules to address unforeseen challenges? What are the current limitations of modular designs in this context, and how could future advancements improve their adaptability?

<span class="date">02/06</span> <span class="topic">Use Case: Navigating US Disaster Recovery Bureaucracy</span> - [Jeffrey Schlegelmilch](https://ncdp.columbia.edu/about-us/faculty-and-staff/), [National Center for Disaster Preparedness](https://ncdp.columbia.edu/) {% include toggle.html content="Jeff Schlegelmilch is the Director of the National Center for Disaster Preparedness at the Columbia Climate School, as well as the Director of Executive Education and Non-Degree Programs for the Columbia Climate School. He is also an Associate Professor for Professional Practice in Climate. His areas of expertise include public health preparedness, community resilience, and the integration of private and public sector capabilities." %}

* Readings
  * [GAO report on disaster recovery](https://www.gao.gov/products/gao-23-104956) (highlights page is sufficient)
  * [Fema infographic](./files/images/fema.png)
* Questions (use the question as a starting point for discussion on slack)
  * In the absence of wholesale change, how can technology support improving efficiency in the bureaucracy of disaster recovery?

<span class="date">02/11</span> <span class="topic">No Lecture: Project Proposal Submission</span> - Instructors will be around to discuss and provide feedback

<span class="date">02/13</span> <span class="topic">Use Case: Agents in Systems Optimization</span> - [Shreya Shankar](https://www.sh-reya.com/) PhD, UC Berkeley {% include toggle.html content="Shreya Shankar is a PhD student in computer science at UC Berkeley, advised by Dr. Aditya Parameswaran. Her research creates practical tools and frameworks that help people build reliable ML systems, with recent work on declarative interfaces and optimization for unstructured data analysis. Her work appears in top data management and HCI venues like SIGMOD, VLDB, CIDR, CSCW and UIST, and she co-organizes the DEEM workshop at SIGMOD. She is supported by the NDSEG Fellowship. Prior to Berkeley, she worked as an ML engineer after completing her B.S. in computer science at Stanford University. In her free time, she enjoys roasting coffee and is actively trying to reduce her Twitter usage.  " %}

* Readings
  * [DocETL](https://arxiv.org/abs/2410.12189)
  * [Palimpzest](https://arxiv.org/pdf/2405.14696) (cost optimization for LLM-powered data processing)
  * (Optional) [ELEET](https://arxiv.org/abs/2410.22522) (fine-tuning smaller models for optimized query execution)
* Questions (rather than answering these, use the questions as a starting point for discussion on slack)
  1. **Systems**: These systems represent different philosophies about determinism in data processing, both in optimization and execution stages: ELEET aims for deterministic extraction with small models, Palimpzest provides deterministic optimization with non-deterministic execution, and DocETL embraces non-determinism in both optimization (given the agents) and execution. How should we think about reliability and correctness guarantees in these different paradigms?
  2. **Systems**: These systems take different approaches to balancing accuracy vs. cost - DocETL optimizes for accuracy with LLM agents, ELEET uses smaller targeted models, and Palimpzest focuses on cost-effective model orchestration. What engineering principles should guide choosing between these approaches for different use cases? What might a unified framework look like?
  3. **HCI**: In document processing systems like DocETL, LLMs can fail in inconsistent ways - e.g., a single LLM may correctly extract 8 names but miss 2 others from the same document, but extract names from other documents perfectly. Unlike traditional data processing errors that follow patterns (e.g., failing on malformed input), LLM failures seem random and hard to systematize. How should interfaces help users validate results and develop trust, when the underlying operations have this fundamentally unpredictable behavior?
  

<span class="date">02/18</span> <span class="topic">Background: Agent Frameworks</span> - [Phil Calçado](https://philcalcado.com/), [Outropy](https://outropy.ai/) 

* Readings:
  * [Building AI Products](https://philcalcado.com/2024/12/14/building-ai-products-part-i.html)
  * [7 Lessons from building a small-scale AI application](https://www.thelis.org/blog/lessons-from-ai)
  * [Compound AI systems](https://bair.berkeley.edu/blog/2024/02/18/compound-ai-systems/)

* Questions (think about and discuss one or more of these topics on slack))
  * Looking at past transformative technologies like the early internet or mobile applications, we see initial barriers around cost, latency, and complexity—challenges that parallel those of today’s AI agents. What key engineering and scientific breakthroughs enabled these technologies to become practical at scale, and what lessons can we apply to AI agents today?
  * Modern cloud architectures are built around stateless, horizontally scalable services, yet AI agents rely on maintaining context and memory. How can these opposing principles be reconciled when designing scalable AI systems? What emerging architectural patterns might enable both scalability and statefulness?
  * The shift from monolithic models to Compound AI systems—where multiple specialized AI components work together—suggests that system design and integration are becoming as crucial as model capabilities. How does this change the skills required for AI engineering, and what new challenges arise when optimizing multi-agent AI systems?
  
<span class="date">02/20</span> <span class="topic">Background: Foundation Models for Embodied/Physical Agents</span> - [Yunzhu Li](https://yunzhuli.github.io), Columbia {% include toggle.html content="I am an Assistant Professor of Computer Science at Columbia University.  Before joining Columbia, I was an Assistant Professor at UIUC CS. I also spent time as a Postdoc at the Stanford Vision and Learning Lab (SVL), working with Fei-Fei Li and Jiajun Wu. I received my PhD from the Computer Science and Artificial Intelligence Laboratory (CSAIL) at MIT, where I was advised by Antonio Torralba and Russ Tedrake, and I obtained my bachelor's degree from Peking University." %}


<blockquote class="blockquote" p class="ms-5 w-90 text-muted">
<p>
Foundation models, such as GPT-4 Vision, have marked significant achievements in the fields of natural language and vision, demonstrating exceptional abilities to adapt to new tasks and scenarios. However, physical/embodied interaction—such as cooking, cleaning, or caregiving—remains a frontier where foundation models and robotic systems have yet to achieve the desired level of adaptability and generalization.</p>

<p>
In this talk, I will discuss the opportunities for incorporating foundation models into classic robotic pipelines to endow robots/physical agents with capabilities beyond those achievable with traditional robotic tools. The talk will focus on three key improvements in (1) task specification, (2) low-level, and (3) high-level scene modeling. The central idea behind this research is to translate the commonsense knowledge embedded in foundation models into structural priors that can be integrated into robot learning systems. This approach leverages the strengths of different modules (e.g., VLM for task interpretation and constrained optimization for motion planning), achieving the best of both worlds. I will demonstrate how such integration enables robots to interpret instructions provided in free-form natural language, and how foundation models can be augmented with additional memory mechanisms, such as an action-conditioned scene graph, to handle a wide range of real-world manipulation tasks.</p>

<p>
Toward the end of the talk, I will discuss the limitations of the current foundation models, challenges that still lie ahead, and potential avenues to address these challenges</p>
</blockquote>

* Readings
  * https://voxposer.github.io/
  * https://rekep-robot.github.io/
* Questions
  * You’ve already seen numerous practical applications of AI agents powered by foundation models in virtual environments. What do you see as the key opportunities and challenges in extending these capabilities to physical agents, particularly those that interact with the real world through robotic manipulation?
  * Additionally, how do the key considerations and assumptions differ between virtual and physical settings?


<span class="date">02/25</span> <span class="topic">Agent-Ready Systems</span> - Jerry/Nikos/Peter/Eugene/Kostis, Columbia

* Readings
  * See class Slack for paper
* Questions
  * What makes agents different from previous workloads/applications from a systems perspective?
  * Based on what we have seen this semester, other systems capabilities may be useful for agent-ready systems to support?

<span class="date">02/27</span> <span class="topic">Systems: Lineage and Data-flow policies</span> - [Eugene Wu](https://www.eugenewu.net), Columbia

* Readings
  * Easier: [Provenance in data visualizations](https://www.dropbox.com/scl/fi/xivnuyo31tk3110bohmvc/smoke-hilda18.pdf?rlkey=bjtsktnij4bl0i4abwtsg4n4u&e=1&dl=0)
  * Harder: [Smoke](https://arxiv.org/abs/1801.07237)
* Questions 
  * How is provenance useful in the context of agents?


<span class="date">03/04</span> <span class="topic">Human-Agent Interaction.   Lydia Chilton</span> 

* Readings: 
  * [Anthropic: You Don't Need a Framework ](https://www.anthropic.com/research/building-effective-agents)
  * [Generative agents: Interactive simulacra of human behavior](https://dl.acm.org/doi/abs/10.1145/3586183.3606763)
* Questions
  * When is human intervention necessary or beneficial in agent-based systems?


<span class="date">03/06</span> <span class="topic">Models: Neurosymbolic training</span> - [Baishakhi Ray](https://rayb.info), Columbia

* Readings
  1. [SemCoder](https://arxiv.org/pdf/2406.01006)
  2. [C2SAFERRUST](https://arxiv.org/pdf/2501.14257)
* Questions to ponder and discuss **at least the day before the class!!** (e.g., not 10 minutes before class)
  1. How neuro-symbolic training can help?
  2. What is the purpose of neurosymbolic reasoning in agentic workflow? 

<!--<span class="date">03/11</span> <span class="topic">HAI: Hand-offs with humans and context</span> - [Lydia Chilton](https://www.cs.columbia.edu/~chilton/chilton.html), Columbia-->

<span class="date">03/11</span> <span class="topic">Human data for building agents that model our minds</span> - [Danielle Perszyk](https://www.linkedin.com/in/danielleoscillations/), Amazon  {% include toggle.html content="Danielle Perszyk is a cognitive scientist at the Amazon AGI SF Lab leading the human data collection efforts for building agents. She received her PhD from Northwestern, where she studied the developmental and evolutionary origins of human's link between language and thought. Previously, she built human data collection programs for UX research and AI model training at Google and Adept. " %}

* Readings
  * [Testing theory of mind in large language models and humans](https://www.nature.com/articles/s41562-024-01882-z)
  * [Generative Agent Simulations of 1,000 People](https://arxiv.org/abs/2411.10109)  or [watch the talk](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=21cbb61c-5482-4183-ac75-b2810137d4ad)
* Question to discuss **at least the day before class!**
  * What does it mean for an agent to model (understand) human minds?

<span class="date">03/13</span> <span class="workshop topic">No Class!  Attend the Agents for Work workshop on 3/12 (link in slack)</span>

<span class="date">03/25</span> <span class="topic">Agent Planning: RL and MCTS</span> - [Shipra Agrawal](https://www.columbia.edu/~sa3305/), Columbia

* Readings
  * [Combining Q-Learning and Search with Amortized Value Estimates, ICLR 2020](https://arxiv.org/abs/1912.02807)
  * [On the role of planning in model-based deep reinforcement learning, ICLR 2021](https://openreview.net/forum?id=IrM64DGB21)
* Questions to ponder while reading.   Discuss these at least one day BEFORE class!
  * How can we combine reinforcement learning methods (like Q-learning) with planning and search to achieve strong performance under small search budgets?
  * What is the role of planning (vs. learning) in performance of agents? What can we learn from the studies of similar approaches for RL systems such as MuZero? Which insights transfer to Agentic systems and which don’t?

<span class="date">03/27</span> <span class="topic">Use Case: Financial Products</span> - [Raman Jatkar](https://www.linkedin.com/in/raman-jatkar-7942079), Intellect Design

* Readings
  * [Dear IT Departments, Please Stop Trying To Build Your Own RAG](https://pub.towardsai.net/dear-it-departments-please-stop-trying-to-build-your-own-rag-4546b4638273)
  * [Multi-Agent System Patterns in Financial Services: Architectures for Next-Generation AI Solutions](https://community.aws/content/2uDxjoo105xRO6Q7mfkogmOYTVp/multi-agent-system-patterns-in-financial-services-architectures-for-next-generation-ai-solutions)
* Questions to ponder while reading.   Discuss these at least one day BEFORE class!
  * What change management approaches are essential for successful Agent systems adoption in financial institutions?
  * Identify real-world applications of multi-agent systems in financial services - in banking, insurance, and wealth management.
  * What key performance indicators should be used to evaluate the effectiveness of agentic systems in enterprise operations?

<span class="date">04/01</span> <span class="topic">HAI: Process Mining and Agents</span> - [Wil van der Aalst](https://en.wikipedia.org/wiki/Wil_van_der_Aalst) (the father of process mining), RWTH Aachen University

* Readings
  * [W.M.P. van der Aalst. Foundations of Process Discovery.](https://www.vdaalst.com/publications/p1330.pdf)
  * [W.M.P. van der Aalst. Object-Centric Process Mining: Unraveling the Fabric of Real Processes.](https://www.vdaalst.com/publications/p1352.pdf)
* Questions to ponder
  * Consider the following traces in a simplified case-centric event log (each letter refers to an activity and each row refers to a case).
    A case could represent the treatment of a patient, the production of a car, or the handling of an invoice. To minimize notation, we use just letters for individual activities. Note that each case starts with activity “a” (e.g., “register patient”) and ends with activity “h” (e.g., “invoice patient”). Assume that all shown traces are frequent (e.g., occur at least 10 times). What process model would you like your discovery technique to discover? Use a Petri net, BPMN model, process tree, or DFG to describe the underlying process.

```
    abcdefgh
    abecfgdh
    abecfdgh
    aebcdfgh
    aebcfgdh
    abcedfgh
    abecdfgh
    aebcfdgh
    abcefgdh
    abcefdgh
    ...
```


<span class="date">04/03</span> <span class="topic">Use Case: Coding (AutoCodeRover)</span> - [Yuntong Zhang](https://yuntongzhang.github.io/), NUS {% include toggle.html content="Yuntong Zhang is a fourth-year PhD student at the National University of Singapore, advised by Prof. Abhik Roychoudhury. His research focuses on LLMs for software engineering, particularly the intersection of program analysis and LLMs for automatic programming. Through his work on the LLM agent AutoCodeRover, he co-founded a spin-off on AI-based coding, which was later acquired by SonarSource." %}


* Readings
  * [AutoCodeRover: Autonomous Program Improvement](https://arxiv.org/abs/2404.05427)
  * [SpecRover: Code Intent Extraction via LLMs](https://arxiv.org/abs/2408.02232)
* Questions to ponder while reading.   Discuss these at least one day BEFORE class!
  * What strategies can be employed to improve the acceptability and trustworthiness of code generated by LLM agents?


<span class="date">04/08</span> <span class="topic">Opportunities and Challenges in Building Agentic Products for Commerce</span> - [Shankar Bhargava](https://www.linkedin.com/in/shankarbhargava/), WalmartLabs

* Readings
  * [Musings About the Future of Search: A Return to the Past?](https://arxiv.org/pdf/2412.18956)
  * [Toward an evaluation science for generative AI systems](https://arxiv.org/pdf/2503.05336)
* Questions to ponder
  * How are agentic systems changing how people search? Has your own usage of Google changed in the past year. How do you think this will change how people shop?
  * Based on what you have learnt in this course so far, what do you think are the challenges in building reliable agentic products for consumers? What are some good metrics to evaluate a consumer shopping agent or assistant?

<span class="date">04/10</span> <span class="topic">The second half</span> - [Shunyu Yao](https://ysymyth.github.io/), OpenAI {% include toggle.html content="Shunyu Yao is a researcher at OpenAI. Previously, he finished his PhD from Princeton. He co-invented some of the most influential and widely used agent methods (ReAct, Tree of Thoughts, Reflexion) and benchmarks (WebShop, SWE-bench, tau-bench), along with OpenAI’s first two agent products (Operator, deep research)." %}

* Readings
  * [SWE-bench](https://arxiv.org/abs/2310.06770) again!
  * [tau-bench](https://arxiv.org/abs/2406.12045)
* Questions to ponder while reading. Discuss these at least one day BEFORE class!
  * In your opinion, what should be the main benchmark to reflect AI’s progress?

<span class="date">04/15</span> <span class="topic">Text2SQL: Compound AI Systems for Querying Structured Data</span> - [Fatma Ozcan](https://techsysinfra.google/research/srg-staff/fatma-ozcan/), Google Research {% include toggle.html content="Fatma Ozcan is a Principal Engineer at Systems Research@Google. Before that, she was a Distinguished Research Staff Member and a senior manager at IBM Almaden Research Center. Her current research focuses on LLMs and ML for data management, text2SQL and conversational interfaces to data, platforms and infrastructure for large-scale data analysis. Dr Ozcan got her PhD degree in computer science from University of Maryland, College Park. She has over 23 years of experience in industrial research, and has delivered core technologies into various IBM products. She has been a contributor to various SQL standards, including SQL/XML, SQL/JSON and SQL/PTF. She is the co-author of the book Heterogeneous Agent Systems, and co-author of several conference papers and patents. She serves on the CRA board of directors, and is the co-chair of CRA-Industry. She received the VLDB Women in Database Research Award in 2022. She is an ACM Fellow and the vice chair of ACM SIGMOD." %}

* Readings
  * [ChaseSQL](https://arxiv.org/pdf/2410.01943)
  * [Is Long Context All You Need?](https://arxiv.org/abs/2501.12372)

<span class="date">04/17</span> <span class="topic">Jailbreaking Large Language Models</span> - [Weiliang Zhao](https://www.cs.columbia.edu/~wz2665/weiliang.html), Columbia

* Readings
  * [Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/pdf/2307.15043)
  * [Diversity Helps Jailbreak Large Language Models](https://drive.google.com/file/d/1qdXsGQcCOAzOU-4wSLWuDVOwMId6_Ejp/view?usp=drive_link)
* Questions to ponder while reading. Discuss these at least one day BEFORE class!
  * Can you think of a way to defend against these approaches?
  * What evaluation criteria should be considered before a model is deployed?


<span class="date">04/22</span> <span class="topic">Delivering knowledge to LLM inference engines via LMCache</span> - [Kuntai Du](https://kuntaidu.github.io/aboutme.html), UChicago {% include toggle.html content="Kuntai Du is a 6th year PhD candidate from University of Chicago, advised by Professor Junchen Jiang. His research focuses on distributed tensor transmission for deep learning model serving systems. Beyond his academic work, he open-sources his research through LMCache and collaborates closely with Professor Ion Stoica and the UC Berkeley team to integrate it into the most popular LLM inference engine vLLM." %}

* Readings 
  * [CacheGen: KV Cache Compression and Streaming for Fast Large Language Model Serving](https://dl.acm.org/doi/10.1145/3651890.3672274)
  * [CacheBlend: Fast Large Language Model Serving for RAG with Cached Knowledge Fusion](https://dl.acm.org/doi/10.1145/3689031.3696098)
* Questions to ponder
  * Should LLMs continuously learn after deployment? If so, what would be a promising way?
 
<span class="date">04/24</span> <span class="topic">Model Context Protocol</span> - Elie Schoppik, Anthropic {% include toggle.html content="Elie Schoppik leads live education at Anthropic as their Head of Technical Training. He has spent over a decade in technical education, working with multiple coding schools and starting one of his own. With a background in consulting, education, and software engineering, Elie brings a practical approach to teaching Software Engineering and AI. He's shared his insights at a variety of technical conferences as well as universities including MIT, Wharton, and UC Berkeley." %}



* Readings
  * [Introducing the Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)
  * [Announcing the Agent2Agent Protocol (A2A)](https://developers.googleblog.com/en/a2a-a-new-era-of-agent-interoperability/)
  * [Model Context Protocol has prompt injection security problems](https://simonwillison.net/2025/Apr/9/mcp-prompt-injection/)
* Questions to ponder
  * Is there really a difference between MCP and A2A and (if so) what do you think it is?

### What You Did

<span class="date">04/29</span> <span class="topic">Presentations</span>

<span class="date">05/01</span> <span class="topic">Presentations</span>



<style>
h3 {
  color: #067832;
  margin-top: 1em;
  margin-bottom: 1em;
}
.date {
color: gray;
background-color: #999;
background-color: #d4f1cc;
color: black;
padding: 2px 6px;
border-radius: 4px;
margin-right: .5em;

}
span.topic {
font-weight: bold;
}
.workshop, .workshop a {
text-transform: uppercase;
}
</style>
