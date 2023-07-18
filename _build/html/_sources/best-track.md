# Best track data

The article notes that data was obtained from a NOAA NHC best-track file.  The link provided does not work.  Now what?

## Finding the data
Luckily, NOAA is not too difficult to find.  See the following (draft) video that does a screen capture of finding and downloading best track data. The video has no sound.  

<div style="width:50vw">
<div class="shiny">
  <iframe class="responsive-iframe" src="https://www.youtube.com/embed/dmcSrs7ZOZs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>
</div>

</br>

Here is a summary of what is shown in the video:
- Do a Google search with key words *NOAA NHC hurricane best track*.   
- I selected the first one I saw: **NHC Data Archive-National Hurricane Center**.
- Click **Best Track Data (HURDAT2)**.
- The first item under Best Track Data is **Atlantic hurricane database** followed by a download link to data in CSV format.  Clicking on the link shows the data in the browser window.  We may use that later, but skip downloading it for now.
- Scroll down to **Tropical Cyclone GIS Data Format**.  
- Click **[archive of GIS data](https://www.nhc.noaa.gov/gis/)**
- Find **Preliminary Best Track**, and click Final Best Tracks **[available here](https://www.nhc.noaa.gov/data/tcr/)**.
- We are following the 2020 Hurricane Sally.  Choose **[2020](https://www.nhc.noaa.gov/data/tcr/index.php?season=2020&basin=atl)**, then scroll down to Sally.
- Before downloading, create a directory just for this project.
- Right-click and download the PDF, KMZ, and SHP to your directory. Later, we'll use this data for our research.  

The video also shows a demo for NOAA's online tool for looking at best track data.

## Look for existing data analysis tools

Never reinvent the wheel.  Before writing your own application to look at data, check out which tools are already available.  In this case:
- [NOAA's Historical Hurricane Tracks](https://www.coast.noaa.gov/hurricanes)

## Was that reproducible?
When referencing data collections in an article, keep in mind that links can change. Check if the data has *persistent identifier*, and if not, provide as much information as you can.  

To ensure your work is reproducible to others, first make sure you can reproduce it yourself! Double check all instructions, no matter how trivial they seem to be.

Here's an example of how simple things go wrong:
- When following the video to create written instructions, I got two CloudFront errors.  CloudFront is AWS's content delivery network(CDN). The error message is listed below.  I had to 'Try again later'.
- The first draft of this page included the actual links to the NHC and HURDAT, but when testing, I found the links worked if I typed them in the browser or used Google, but they were blocked when clicking from my draft website.  

Data providers distribute their content across the globe, so it makes sense they may have a hiccup or two. Data providers need to protect their servers, so it makes sense to limit or block certain access points. Understanding a bit about how data is hosted, (a topic for later), will help you find patience and hopefully encourage you to provide more details on how to access the data needed to reproduce your work.

## Prepare for Open Science
To make sure the next researcher can find and replicate *your* results, check in with [TOPS Core Open Science Skills](https://nasa.github.io/Transform-to-Open-Science-Book/Open_Science_Cookbook/Your_Open_Science_Journey.html#section-1-core-open-science-skills).  If you haven't already, take a break and knock out the following:
- [Get an ORCID](https://nasa.github.io/Transform-to-Open-Science-Book/Open_Science_Cookbook/Your_Open_Science_Journey.html#get-an-orcid)
- [Get a GitHub](https://nasa.github.io/Transform-to-Open-Science-Book/Open_Science_Cookbook/Your_Open_Science_Journey.html#get-a-github)
- [Get a Zenodo Account](https://nasa.github.io/Transform-to-Open-Science-Book/Open_Science_Cookbook/Your_Open_Science_Journey.html#get-a-zenodo-account)

## Acronyms and notes 
- AWS - Amazon Web Services
- CSV - Comma Separated Values
- GIS - Geographic Information Systems
- HURDAT2 - Hurricane Database, 2nd generation
- KMZ - Keyhole Markup Language, a file format used to display information on maps
- NHC - National Hurricane Center 
- NOAA - National Oceanic and Atmospheric Administration 
- ORCID - Open Researcher and Contributor ID
- PDF - Portable Document Format
- SHP - In this case, SHP was just the name of the link to download a shapefile, which is a collection of GIS files. The main file has suffix *.shp*.
- TOPS - Transform to Open Science

The CloudFront error was:
```
421 ERROR
The request could not be satisfied.
The distribution does not match the certificate for which the HTTPS connection was established with. 
We can't connect to the server for this app or website at this time. There might be too much traffic 
or a configuration error. Try again later, or contact the app or website owner.
If you provide content to customers through CloudFront, you can find steps to troubleshoot and help 
prevent this error by reviewing the CloudFront documentation.
Generated by cloudfront (CloudFront)
Request ID: 5u6TaJlmajq5Blanz3bNXm2V_Hz8l2LRHrc4B7dIMdWg4ydpp-BqPQ==
```

## Other ways to get HURDAT2 data

Compiling a list...
- [Google Earth Engine Data Catalog](https://developers.google.com/earth-engine/datasets/catalog/NOAA_NHC_HURDAT2_atlantic).  Free to use for research, education, and nonprofit use, requires users to sign up for Earth Engine access.


