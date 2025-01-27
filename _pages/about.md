---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm currently a researcher/software engineer at Computing Infrastructure Lab of Bytedance Inc. My current work focuses on building next-generation AI serving infrastructures. Previously I was a Postdoc Researcher of Computer Science at UT Austin, working with [Prof. Aditya Akella](http://pages.cs.wisc.edu/~akella/) at UT Networked Systems group ([UTNS](https://utns.cs.utexas.edu/)). I was one of the recipients of [CIFellow 2021](https://cifellows2021.org/2021-class/), supported by both National Science Foundation (NSF) and Computing Research Association (CRA). During my PhD I worked on making real time data processing systems more elastic, under the supervision of [Prof. Indranil Gupta](http://indy.cs.illinois.edu/) at Distributed Protocols Research Group ([DPRG](http://dprg.cs.uiuc.edu/)). My current research mainly revolves around all aspects of resource-efficient cloud computing frameworks, including serverless computing and alternative system architectures. See my [CV]() and list of [publications](https://scholar.google.com/citations?user=uFyE-AQAAAAJ) here.
Don't hesitate to [contact me](le.xu@bytedance.com) if you're interested in my experience or would like to chat about my recent research! I'm always open to opportunities for collboration and/or full-time research positions.


Education
======
* Ph.D. in Computer Science, University of Illinois at Urbana Champaign, 12/2021
  * Advised by Indranil Gupta.
  * Thesis: [Elastic techniques to handle dynamism in real-time data processing systems](https://www.ideals.illinois.edu/items/123174/bitstreams/405779/data.pdf)
* M.S. in Computer Science, University of Illinois at Urbana Champaign, 05/2015
  * Advised by Indranil Gupta.
* B.S. in Math and Computer Science, University of Illinois at Urbana Champaign, 05/2013

Publications and Preprints
======
* **[Preprints]** Bodun Hu, Jiamin Li, Le Xu, Myungjin Lee, Akshay Jajoo, Geon-Woo Kim, Hong Xu, Aditya Akella “*<u>BlockLLM: Multi-tenant finer-grained serving for large language models</u>*” [[arxiv]](https://arxiv.org/pdf/2404.18322)
  * A block-based LLM serving framework for fine-grained resource provisioning.
* **[Preprints]** Le Xu, Divyanshu Saxena, Neeraja J. Yadwadkar, Aditya Akella and Indranil Gupta. “*<u>Dirigo: Self-scaling Stateful Actors For Serverless Real-time Data Processing.</u>*” [[arxiv]](https://arxiv.org/abs/2308.03615)
  * A virtual actor model that helps stream processing applications to scale freely at fine granularity.
* **[EMNLP 24]** Bodun Hu, Le Xu, Jeongyoon Moon, Neeraja J. Yadwadkar, Aditya Akella. “*<u>MOSEL: Inference Serving Using Dynamic Modality Selection.</u>*” [[link]](https://aclanthology.org/2024.emnlp-main.501.pdf)
  * A modality-selection framework for real-time ML inference for multi-modality data.  
* **[IROS 23]** Peter Schafhalter, Sukrit Kalra, Le Xu, Joseph E. Gonzalez, and Ion Stoica. “*<u>Leveraging Cloud Computing to Make Autonomous Vehicles Safer.</u>*” [[link]](/files/IROS23_2514_FI.pdf) [[arxiv]](ttps://arxiv.org/abs/2308.03204)
  * A systematic approach that improves driving safety for autonomous vehicles with the unreliable resource pool of the cloud. 
* **[VLDB 22]** Li Su, Xiaoming Qin, Zichao Zhang, Rui Yang, Le Xu, Indranil Gupta, Wenyuan Yu, Kai Zeng and Jingren Zhou. “*<u>Banyan: A Scoped Dataflow Engine for Graph Query Service.</u>*” [[link]](https://www.vldb.org/pvldb/vol15/p2045-su.pdf) [[arxiv]](https://arxiv.org/abs/2202.12530)
  * A scoped dataflow model for graph traversal queries that explicitly exposes concurrent execution and control of any subquery to the finest granularity. 
* **[PhD Thesis]** Le Xu. “*<u>Elastic techniques to handle dynamism in real-time data processing systems.</u>*” [[link]](https://www.ideals.illinois.edu/items/123174/bitstreams/405779/data.pdf)
* **[NSDI 21]** Le Xu, Shivaram Venkataraman, Indranil Gupta, Luo Mai, and Rahul Potharaju. “*<u>Move Fast and Meet Deadlines: Fine-grained Real-time Stream Processing with Cameo.</u>*” [[link]](files/nsdi21-xu.pdf) [[arxiv]](https://arxiv.org/abs/2010.03035) [[slides]](files/nsdi21_slides_xu.pdf) [[video]](https://www.youtube.com/watch?v=V_DyLNG0Crg)
  * A performance target-aware scheduling frameowrk that supports fine-grained operator scheduling, built for actor-based, distributed dataflow runtime. 
* **[CODASPY 20]** Long, Yunhui, Le Xu and Carl A. Gunter. “*<u>A Hypothesis Testing Approach to Sharing Logs with Confidence.</u>*” [[link]](files/log-obfuscation-cr.pdf) 
  * An end-to-end framework that allows users to identify risks of information leakage in logs, and to release the logs with a much lower risk of exposing the sensitive attribute through log obfuscation.
* **[SoCC 18]** Kalim, Faria, Le Xu, Sharanya Bathey, Richa Meherwal, and Indranil Gupta. “*<u>Henge: Intent-driven Multi-Tenant Stream Processing</u>*” [[link]](files/henge-cr.pdf) [[slides]](files/Henge-SoCC2018.pptx) [[arxiv]](https://arxiv.org/abs/1802.00082)
  * An intent-driven mechanism to unify user-defined performance objectives and improve cluster-wise overall satisfaction in multi-tenant stream processing system.
* **[VLDB 18]** Luo Mai, Kai Zeng, Rahul Potharaju, Le Xu, Steve Suh, Shivaram Venkataraman, Paolo Costa, Terry Kim, Saravanan Muthukrishnan, Vamsi Kuppa, Sudheer Dhulipalla, and Sriram Rao. “*<u>Chi: a scalable and programmable control plane for distributed stream processing systems.</u>*” [[link]](files/chi-cr.pdf) [[slides]](files/chi-vldb2018.pptx) 
  * A generalized control plane and control message design for stream processing systems that allows a wide range of functionalities being implemented and efficiently executed.
* **[EuroSys 18]** Mainak Ghosh, Ashwini Raina, Le Xu, Xiaoyao Qian, Indranil Gupta, and Himanshu Gupta. “*<u>Popular is Cheaper: Curtailing Memory Costs in Interactive Analytics Engines.</u>*” [[link]](files/Getafix_ShepherdVersion.pdf) [[slides]](files/getafix.pptx) [[tech report]](files/getafix-tr.pdf)
  * Replication and routing strategy designed for popularity-driven workloads for interactive analytics engines.
* **[SoCC 2017]** Mijung Kim, Jun Li, Haris Volos, Manish Marwah, Alexander Ulanov, Kimberly Keeton, Joseph Tucek, Lucy Cherkasova, Le Xu, and Pradeep Fernando. “*<u>Sparkle: Optimizing spark for large memory machines and analytics</u>*” [[link]](https://dl.acm.org/doi/abs/10.1145/3127479.3134762) [[arxiv]](https://arxiv.org/abs/1708.05746)  
  * A shared-memory shuffle engine and off-heap memory store that optimize Spark in the scale-up setting.
* **[IC2E 2016]** Le Xu, Boyang Peng, and Indranil Gupta. “*<u>Stela: Enabling stream processing systems to scale-in and scale-out on-demand.</u>*” [[link]](files/PID4058711.pdf) [[slides]](files/stela-final-copy.pptx) [[video]](https://www.youtube.com/watch?v=RqFO1fLQAr4) 
  * Exploring topology-aware algorithms for migrating real time tasks to optimize distributed stream processing system throughput during cluster configuration changes.
* **[Master Thesis]** Le Xu. “*<u>Stela: on-demand elasticity in distributed data stream processing systems.</u>*” [[link]](files/XU-THESIS-2015.pdf)
* **[IWCA 2015]** Wenting Wang, Le Xu, and Indranil Gupta. "Scale Up vs. Scale Out in Cloud Storage and Graph Processing Systems. “*<u>Stela: Enabling stream processing systems to scale-in and scale-out on-demand.</u>*” [[link]](files/scaleOutUp.pdf) [[slides]](files/presentation.pptx)  
  * Constructing cluster's linear pricing model for both scale up and scale out cluster based on pricing scheme provided by major cloud providers.


Industrial Experiences
======
* **[June 2019 - Aug 2019]**:  Research Intern -- Alibaba Damo Academy (Data Analytics and Intelligence Lab)
  * Building hierarchical actor-based framework for distributed graph querying service.
  * Supervisor: Kai Zeng

* **[May 2017 - Aug 2017]**:  Research Intern -- Microsoft (Cloud and Information Services Lab)
  * Building a control layer inside of a real-time stream processing engine for flexible and efficient online monitoring and re-configuration.
  * Supervisor: Kai Zeng, Rahul Potharaju

* **[May 2016 - Aug 2016]**: Research Intern -- Hewlett-Parkard Labs (Software Analytics Group)
  * Conducting Spark performance analysis for micro-benchmark and machine learning applications
  * Supervisor: Mijung Kim, Jun Li
  
<!-- Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3 -->


<!-- Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul> -->
  
Teaching
======
**[05/2018, 05/2020]**: Teaching Assistant: Cloud Computing Capstone (Coursera)

**[01/2015, 09/2019]**: Teaching Assistant: Distributed System (CS 425)

**[01/2015, 01/2016]**: Teaching Assistant: Cloud Computing Concepts (Coursera) 

**[01/2016]**: Teaching Assistant: Advanced Distributed Systems (CS 525) 


Service and leadership
======
**[Program Committee]**: 2024 USENIX Symposium on Networked Systems Design and Implementation (NSDI 24')

**[Program Committee]**: 2023 ACM/IFIP/USENIX International Middleware Conference (Middleware 23') 

Honors, Memberships, Awards
======
* 2021: 2021 CRA/CCC Computing Innovation Fellows
* 2020: Rising Stars EECS Workshop
* 2019: SOSP 19 Travel Grant
* 2018: OSDI 18 Travel Grant
* 2018: SoCC 18 Travel Grant
* 2017: SOSP 17 Travel Grant
* 2016: David J. Kuck Outstanding M.S. Thesis Award
* 2015: Grace Hopper Celebration Travel Fund
* 2015: Conference Travel Grant
* 2015: Outstanding Teaching Assistant
* 2011: Member of PI MU EPSILON: National Math Honor Society 
* 2010: Edmund J James Scholar

Cloud-Free Zone
======
* Sometimes I blah about random thoughts. ATTENTION: you are about to enter a [cloud-free zone](https://happyandslow.wordpress.com)!
* Occationally I [tweet](https://twitter.com/happyandslow) (or retweet) about things (those are not entirely cloud-free).


<!-- This is the front page of a website that is powered by the [Academic Pages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html). -->

<!-- Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
3. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
4. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
5. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
6. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
