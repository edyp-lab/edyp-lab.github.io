---
layout: project
title: mzdbConverter
see_also: "true"
web_home: "http://www.profiproteomics.fr/proline"
github_project: "**https://github.com/edyp-lab/msDataConverter**"
url_download: "http://www.profiproteomics.fr/proline-downloads/"
---
<br>
Command line tool to convert Thermo ".raw" files or Brucker ".d" directories to mzdb files.   
<br>
<a href="/images/mzdb_convert.png" target="_blank">
    <img src="/images/mzdb_convert.png" class="screenshot" />
</a>
<br>
For Thermo raw files : 
<a href="/images/mzdb_convert_thermo.png" target="_blank">
    <img src="/images/mzdb_convert_thermo.png" class="screenshot" />
</a>
<br>
For Brucker .d folders :
<a href="/images/mzdb_convert_brucker.png" target="_blank">
<img src="/images/mzdb_convert_brucker.png" class="screenshot" />
</a>

* The main repository creates the final distribution but it includes other modules, see description below.

## msDataConverter
**Public**

Main repository 


## msDataConsumer
**Private**  

This module is used to get msData information in order to process it.
<br>The module starts a Socket Server on specific port, and delegated process to appropriated consumer
* to mzdb writer to convert msData to mzdb File.
* to metadata controller to create acquisition file Metadata for callbacks implementations 
 
* Repository [msDataConsumer](https://github.com/edyp-lab/msDataConsumer) 

## ThermoAccess 
**Private**  

This module, written in C#, is a Thermo Fisher raw file reader. It used ThermoFisher.CommonCore package.
<br>
The read data is sent on serializer socket server, unless read-only parameter is specified 

* Repository [ThermoAccess](https://github.com/edyp-lab/ThermoAccess) 

<br>
Several projects deal with file formats and their conversion or generation.  
See repositories with [*fileformats* topics](https://github.com/search?q=topic%3Afileformats+org%3Aedyp-lab+fork%3Atrue&type=repositories)
