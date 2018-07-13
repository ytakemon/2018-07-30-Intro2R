---
layout: workshop      # DON'T CHANGE THIS.
carpentry: ""    # what kind of Carpentry (must be either "lc" or "dc" or "swc")
venue: "Introduction to the R programming"        # brief name of host site without address (e.g., "Euphoric State University")
address: "159 Old Bar Harbor Rd, Bar Harbor"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "us"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "44.432094,-68.290329"       # decimal latitude and longitude of workshop venue (e.g., "41.7901128,-87.6007318" - use http://www.latlong.net/)
humandate: "July 30th-Aug 1st, 2018"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "1:00 pm - 4:00 pm"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2018-07-30      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2018-07-31        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Yuka Takemon"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["George Sutphin", "Ron Korstanje"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["yuka.takemon@jax.org"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes:             # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document
eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
---
<h2 id="general">General Information</h2>

  This workshop is intended for those with limited or no experience in the R language and/or any form of coding language. We will work towards becoming familiar with how to read and write data, types of data structures, data manipulation, and other forms of general utilities that can help speed up data processing and analyses.

  Our goal is to introduce (new) concepts and vocabulary, and most importantly exposure to working in R.

  We encourage those with coding experience (python, C, C++, unix, etc.) to help your neighbours!

<p id="requirements">
  <strong>Requirements:</strong> Participants must bring a laptop with a
  Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges
  on. They should have a few specific software packages installed (listed
  <a href="#setup">below</a>).
</p>

<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.email %}
    {% for email in page.email %}
      {% if forloop.last and page.email.size > 1 %}
        or
      {% else %}
        {% unless forloop.first %}
        ,
        {% endunless %}
      {% endif %}
      <a href='mailto:{{email}}'>{{email}}</a>
    {% endfor %}
  {% else %}
    to-be-announced
  {% endif %}
  for more information.
</p>

<hr/>

{% comment %}
  SCHEDULE

  Show the workshop's schedule.  Edit the items and times in the table
  to match your plans.  You may also want to change 'Day 1' and 'Day
  2' to be actual dates or days of the week.
{% endcomment %}

<h2 id="schedule">Schedule</h2>

<div class="row">
<div class="col-md-6">
<h3>Monday, July 30th</h3>
<table class="table table-striped">
<tr> <td>01:00</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/">Workshop Overview</a> </td></tr>
<tr> <td>01:10</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/01-rstudio-intro/">Introduction to R and RStudio</a> </td></tr>
<tr> <td>01:20</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/02-project-intro/">Project management</a> </td></tr>
<tr> <td>01:40</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/03-seeking-help/">Seeking help</a> </td></tr>
<tr> <td>01:50</td>  <td> <a href="http://swcarpentry.github.io/shell-novice/02-filedir/index.html">Navigating files and directories</a> </td></tr>
<tr> <td>02:00</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/15-knitr-markdown/">Producing reports with knitr</a> </td></tr>
<tr> <td>02:30</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/04-data-structures-part1/">Understanding data structures</a> </td></tr>
<tr> <td>03:15</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/05-data-structures-part2/">Exploring data frames</a> </td></tr>
<tr> <td>03:45</td> <td>Wrap-up</td></tr>
</table>

<h3>Tuesday, July 31st</h3>
<table class="table table-striped">
<tr> <td>01:00</td>  <td>Recap</td></tr>
<tr> <td>01:15</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/07-control-flow/">Control flow</a> </td></tr>
<tr> <td>02:00</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/10-functions/">Creating functions</a> </td></tr>
<tr> <td>02:45</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/08-plot-ggplot2/">Publication quality graphics</a> </td></tr>
<tr> <td>03:30</td>  <td> <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/11-writing-data/">Writing data</a> </td></tr>
<tr> <td>03:45</td>  <td>Wrap-up</td></tr>
</table>
</div>
</div>

{% if page.collaborative_notes %}
<p id="collaborative_notes">
  We will use this <a href="{{page.collaborative_notes}}">collaborative document</a> for chatting, taking notes, and sharing URLs and bits of code.
</p>
{% endif %}

We will use this <a href="https://drive.google.com/open?id=1g4yI-JSKs7N1_-TQ-EvuILMdJ6gjvCSb">Google Drive</a> to get our data and work collaboratively in the google doc. The <a href="https://docs.google.com/document/d/1-LaIKEPOCyOmYuAEKDYrRxL8oYS7XRQYZQiVia1PowM/edit?usp=sharing">Google Doc</a> will be used for chatting, taking notes, and sharing URLs and bits of codes.

<hr/>

<h2 id="setup">Setup</h2>

<p>
  To participate in a
  {% if page.carpentry == "swc" %}
  Software Carpentry
  {% elsif page.carpentry == "dc" %}
  Data Carpentry
  {% elsif page.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need access to the software described below.
  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>
<div id="r"> {% comment %} Start of 'R' section. {% endcomment %}
  <h3>R</h3>

  <p>
    <a href="http://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="http://www.rstudio.com/">RStudio</a>.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="r-windows">Windows</h4>
      <a href="https://www.youtube.com/watch?v=q0PjTAylwoU">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
        Note that if you have separate user and admin accounts, you should run the
        installers as administrator (right-click on .exe file and select "Run as
        administrator" instead of double-clicking). Otherwise problems may occur later,
        for example when installing R packages.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-macosx">macOS</h4>
      <a href="https://www.youtube.com/watch?v=5-ly3kyxwEg">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-linux">Linux</h4>
      <p>
        You can download the binary files for your distribution
        from <a href="http://cran.r-project.org/index.html">CRAN</a>. Or
        you can use your package manager (e.g. for Debian/Ubuntu
        run <code>sudo apt-get install r-base</code> and for Fedora run
        <code>sudo dnf install R</code>).  Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
  </div>
</div>


<h2 id="attribution">Attribution</h2>
<p>
This website is derived from the <a href="{{site.workshop_site}}">Software Carpentry Workshop Template</a>
under a <a href="https://ytakemon.github.io/2018-07-30-MDIBL-CompAging-Intro2R/LICENSE.html">Creative Commons Attribution (CC BY 4.0) License</a>.
Changes were made to branding and some content.
</p>
