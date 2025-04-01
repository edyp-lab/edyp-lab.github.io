---
layout: project
title: ePims
img_project : "/images/epims1.png"
see_also: "true"
github_project: "https://github.com/edyp-lab/epims-server"
url_help: "http://biodev.extra.cea.fr/docs/epims"
---
<br>
ePims is a LIMS (Laboratory Information Management System) dedicated to Proteomics data, in particular mass spectrometry data.  
 It provides activity monitoring and traceability of electronic data related to proteomic mass spectrometry analyses.
<br>

Download, support and details will be available soon. 

## Repositories

Git repositories are currently hosted on [CEA Tuleap](https://codev-tuleap.intra.cea.fr/projects/epims).   
Code migration is in progress...

ePims is organized into 5 repositories:

* epims-server&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/epims-server" target="_blank"><i class="fa fa-github"></i></a>
  * Server side of ePims. Rest and JMS server linked to ePims database. 
* epims-client&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/epims-client" target="_blank"><i class="fa fa-github"></i></a>
  * Activity, Sample and Instrument Management GUI Application. To be used by ePims user to access to epims-server
* epims-epback&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/epims-epback" target="_blank"><i class="fa fa-github"></i></a>
  * Software used to transfer new acquisitions from an Instrument PC to the ePims repository
* epims-json&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/epims-json" target="_blank"><i class="fa fa-github"></i></a>
  * Libraries of json objects shared between different projects.
* epims-eptaf&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/epims-eptaf" target="_blank"><i class="fa fa-github"></i></a>
  * Software that listens to a JMS file to find out about new acquisitions available on the server.



