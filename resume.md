---
layout: default
title: Resume
permalink: /resume/

education:
  - date: Apr 2016 - Aug 2016
    title: "Bachelor's Degree on Computer Science Engineering, GPA: 9.04/10"
    company: Universidad Complutense de Madrid
    location: Madrid, Spain
    media:
      name: Record
      icon: "fas fa-arrow-circle-down"
      url: "/documents/AnaMariaMartinez-CS-set.pdf"

  - date: Apr 2016 - Aug 2016
    title: "Bachelor's Degree on Mathematics, GPA: 8.11/10"
    company: Universidad Complutense de Madrid
    location: Madrid, Spain
    media:
      name: Record
      icon: "fas fa-arrow-circle-down"
      url: "/documents/AnaMariaMartinez-M-set.pdf"


jobs:
  - date: Sep 2016 - Present
    title: Software Engineer at the Open Build Service Frontend Team
    company: SUSE
    location: Nürenberg, Germany

  - date: Apr 2016 - Aug 2016
    title: Google Summer of Code (Ruby on Rails developer)
    company: openSUSE
    media:
      name: Blog
      icon: "fab fa-wordpress"
      url: "https://gsocwithopensuse.wordpress.com"

  - date: Nov 2015 - June 2016
    title: Fellowship to collaborate in the Computer Architecture Department
    company: Universidad Complutense de Madrid
    location: Madrid, Spain

  - date: June - Aug 2015
    title: Santander SME internship grant (Ruby on Rails developer)
    company: Socialmenta
    location: Madrid, Spain

  - date: Summer 2013, Summer 2014
    title: Leisure time monitor in an English summer camp for children
    company: GADER Formación y Eventos, Utopía XXI
    location: Madrid, Spain

  - date: 2009 - 2014
    title: Chess and English teacher
    company: Collado Villalba Chess Club, Utopía XXI
    location: Madrid, Spain


honors:
  - date: 2016
    title: Excellence Grant for high academic performance university students
    company: Community of Madrid


projects:
  - name: "Open Build Service"
    commits-url: "openSUSE/open-build-service"

  - name: "OSEM"
    commits-url: "openSUSE/osem"

  - name: "Agile Team Dashboard"
    commits-url: "openSUSE/agile-team-dashboard"

  - name: "Trollolo"
    commits-url: "openSUSE/trollolo"

  - name: "Rantly"
    commits-url: "rantly-rb/rantly"

  - name: "Ruby Core"
    prs-url: "ruby/ruby"

  - name: "obs-landing"
    commits-url: "openSUSE/obs-landing"

  - name: "Rubocop"
    commits-url: "bbatsov/rubocop"

  - name: "HAML-Lint"
    commits-url: "brigade/haml-lint"

  - name: "Git Cop"
    prs-url: "bkuhlmann/git-cop"

  - name: "coala-bears"
    commits-url: "coala/coala-bears"

  - name: "CONSUL"
    commits-url: "consul/consul"


my_projects:
  - name: "Android app to collect medical data"
    project-url: "Ana06/medical-data-android"

  - name: "Machine learning algorithms in Python"
    project-url: "vicgalle/machine-learning"

  - name: "Solution of ODE with MATLAB"
    project-url: "Ana06/ode"

  - name: "Computer Algebra algorithms in Maple"
    project-url: "Ana06/comp-algebra"

  - name: "A C-like language compiler to Pascal in Java"
    project-url: "Ana06/C-like-compiler"

  - name: "Interactive prototype of a messaging mobile app"
    url: "http://www.youtube.com/watch?v: iCR0IikbKpw"

  - name: "Text decoder written in Haskell"
    project-url: "https://github.com/consul/consul/commits?author: Ana06"

  - name: "The Connect Four game implemented in C++"
    project-url: "Ana06/contact4"

  - name: "Artificial Intelligence projects (Prolog, Jess, Protégé)"
    project-url: "Ana06/AI"

  - name: "Function graphing with VHDL over a FPGA"
    project-url: "Ana06/function-graphing-FPGA"
---

<h1 class="text-center title">{{ page.title | escape }}</h1>
<hr class="title">

{% include resume/experience.html title="Education" jobs=page.education %}
{% include resume/experience.html title="Experience" jobs=page.jobs %}

{% include resume/honors.html %}

{% include resume/contributions.html %}

