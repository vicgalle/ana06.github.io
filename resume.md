---
layout: default
title: Resume
permalink: /resume/

education:
  - date: Sep 2011 - July 2016
    title: "Bachelor's Degree on Computer Science Engineering, GPA: 9.04/10"
    company: Universidad Complutense de Madrid
    location: Madrid, Spain
    featured: true
    media:
      name: Record
      icon: "fas fa-arrow-circle-down"
      url: "/documents/AnaMariaMartinez-CS-set.pdf"

  - date: Sep 2011 - July 2016
    title: "Bachelor's Degree on Mathematics, GPA: 8.11/10"
    company: Universidad Complutense de Madrid
    location: Madrid, Spain
    featured: true
    media:
      name: Record
      icon: "fas fa-arrow-circle-down"
      url: "/documents/AnaMariaMartinez-M-set.pdf"

  - date: Sep 2009 - June 2011
    title: "Technological Baccalaureate, Graduated with Honors"
    company: IES Lázaro Cárdenas
    location: Madrid, Spain


jobs:
  - date: Sep 2016 - Present
    title: Software Engineer at the Open Build Service Frontend Team
    company: SUSE
    location: Nürenberg, Germany
    featured: true

  - date: Apr 2016 - Aug 2016
    title: Google Summer of Code (Ruby on Rails developer)
    company: openSUSE
    featured: true
    media:
      name: Blog
      icon: "fab fa-wordpress"
      url: "https://gsocwithopensuse.wordpress.com"

  - date: Nov 2015 - June 2016
    title: Fellowship to collaborate in the Computer Architecture Department
    company: Universidad Complutense de Madrid
    location: Madrid, Spain
    featured: true

  - date: June - Aug 2015
    title: Santander SME internship grant (Ruby on Rails developer)
    company: Socialmenta
    location: Madrid, Spain
    featured: true

  - date: Summer 2013, Summer 2014
    title: Leisure time monitor in an English summer camp for children
    company: GADER Formación y Eventos, Utopía XXI
    location: Madrid, Spain
    featured: true

  - date: 2013 - 2014
    title: English teacher
    company: Utopía XXI
    location: Madrid, Spain

  - date: 2009 - 2011
    title: Chess teacher
    company: Collado Villalba Chess Club
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

  - name: "Jekyll"
    commits-url: "jekyll/jekyll"

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

  - name: "mentoring"
    commits-url: "openSUSE/mentoring"

  - name: "Hackweek"
    commits-url: "SUSE/hackweek"

  - name: "software-o-o"
    commits-url: "openSUSE/software-o-o"


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


talks:
  - name: Getting started as an open source contributor 
    conference: openSUSE.Asia Summit 2017 (Tokyo, Japan)
    url: https://events.opensuse.org/conference/summitasia17/program/proposal/1586
    featured: true

  - name: Property testing in Ruby (Lightning Talk)
    conference: Euruko 2017 (Budapest, Hungary)
    url: https://www.youtube.com/watch?v=0bDRKUqIu24&t=18m33s
    featured: true

  - name: OBS in numbers
    conference: openSUSE Conference 2017 (Nurenberg, Germany)
    url: https://events.opensuse.org/conference/oSC17/program/proposal/1388#2
    featured: true
    
  - name: First steps in a Big Data project & MongoDB
    conference: Summer University Complutense school 2016 (Madrid, Spain)
    featured: true

  - name: Virus competition (workshop)
    conference: openSUSE Conference 2017 (Nurenberg, Germany)
    url: https://events.opensuse.org/conference/oSC17/program/proposal/1326

  - name: Property and mutant testing
    conference: Local conferences such as DevOps Camp (Germany)

 
languages:
  - name: Spanish
    certificate: Native speaker
  - name: English
    certificate: C2 - Certificate of Proficiency in English (CPE) by Cambridge University in June 2016
  - name: German
    certificate: B1 - Deutsch-Test für Zuwanderer by telc and BAMF in October 2017
---

<h1 class="text-center title">{{ page.title | escape }}</h1>
<hr class="title">

{% include resume/experience.html title="Education" jobs=page.education type="experience"%}
{% include resume/experience.html title="Experience" jobs=page.jobs type="job"%}

{% include resume/honors.html %}

{% include resume/contributions.html %}

{% include resume/talks.html %}

{% include resume/languages.html %}

<script>
function more(event, elem) {
    event.preventDefault();
    var type = $(elem).data("type");
    $('.no-featured-' + type).toggleClass('hidden');
    if($(elem).text() === 'more')
        $(elem).text('less');
    else
        $(elem).text('more');
}
</script>
