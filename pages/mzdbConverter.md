---
layout: project
title: mzdbConverter / msDataConverter
img_project : "/images/mzdb_convert_banner1.png"
see_also: "true"
web_home: "http://www.profiproteomics.fr/proline"
github_project: "https://github.com/edyp-lab/msDataConverter"
url_download: "https://www.profiproteomics.fr/proline-downloads/#ms_files_toolset"
---
<br>
Command line tool to convert Thermo ".raw" files or Brucker ".d" directories to mzdb files.  
This tools may also be used as an API for development to access some ThermoFisher acquisition metadata 
  
  
Two manufacturer are actually supported: ThermoFisher and Bruker, use *thermo* or *bruker* option respectively.  
The *--help* list options according to the specified input file format (thermo / bruker) 
  
Available options for Thermo Fisher raw files : 
<a href="/images/mzdb_convert_thermo.png" target="_blank">
    <img alt="mzdb_convert help" src="/images/mzdb_convert_thermo.png" class="screenshot" />
</a>
  
Available options for  Bruker .d folders :
<a href="/images/mzdb_convert_brucker.png" target="_blank">
<img alt="mzdb_convert help" src="/images/mzdb_convert_brucker.png" class="screenshot" />
</a>

## Repositories

* msDataConverter&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/msDataConverter" target="_blank"><i class="fa fa-github"></i></a>
  * The main repository creates the final distribution but it includes other modules listed here.
* msDataConsumer&nbsp;&nbsp;<i class="fa fa-grayicon fa-unlock"  title="Public"></i>&nbsp;<a href="https://github.com/edyp-lab/msDataConsumer" target="_blank"><i class="fa fa-github"></i></a>
  * This module is used to get msData information in order to process it. It starts a Socket Server on specific port, and delegated process to appropriated consumer
    * to mzdb writer to convert msData to mzdb File.
    * to metadata controller to create acquisition file Metadata for callbacks implementations 
* ThermoAccess&nbsp;&nbsp;<i class="fa fa-grayicon fa-lock"  title="Private"></i>&nbsp;<a href="https://github.com/edyp-lab/ThermoAccess" target="_blank"><i class="fa fa-github"></i></a> 
  * This module, written in C#, is a Thermo Fisher raw file reader. It used ThermoFisher.CommonCore package. The read data is sent on serializer socket server, unless read-only parameter is specified 

*To be dispatched in files *
<br>
Several projects deal with file formats and their conversion or generation.  
See repositories with [*fileformats* topics](https://github.com/search?q=topic%3Afileformats+org%3Aedyp-lab+fork%3Atrue&type=repositories)
