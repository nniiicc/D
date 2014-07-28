###The Data Usage Index

The first of these studies was an analysis of the user logs from the Research Data Archive (RDA) where ICOADS is hosted and served to end users. In this work, we hoped to develop a set of indicators based on data access events (e.g. downloads, pages visited, etc.) that would allow us to make a more robust set of statements about ICOADS impact than simply saying how many times it had been downloaded. To do this, we borrowed largely from an existing Data Usage Index (DUI) developed in the life sciences \cite{chavan2009towards}; \cite{ingwersen2011indicators}. In adapting the DUI for climate related data procuts we first developed a suite of DUI indicators specific to the types of interaction events of RDA users (see Table 1, more details can be found in Weber et al. 2014).

<br>

| | Code      | Indicator             | Explanation                                                             |
|------|-----------------|---------------------------|--------------------------------------------------------------|
| 1    | uu(ds)          | Unique Users              | Unique users that downloaded data during a time window       |
| 2    | n(ds)           | Number of Datasets        | Number of Datasets assigned DS number by RDA                 |
| 3    | f(ds)           | Files DS                  | Number of files in Dataset per time window                   |
| 4    | d(ds)           | Download Frequency        | Total number of files downloaded per time window             |
| 5    | hp(ds)          | Homepage Hits             | Home Page Hits of Data Set per time window                   |
| 7    | d(ds) /uu (ds)  | Download Density          | Average number of files downloaded per unique user           |
| 8    | d(ds) / f (ds)  | Usage Impact              | Total number of downloaded files over total files in dataset |
| 9    | d(ds) / hp(ds)  | Usage Balance             | Files downloaded by number of homepage hits per time window  |
| 10   | hp(ds) / f(ds)  | Interest impact           | Total homepage hits per number of files in dataset           |
| 11   | hp(ds) / uu(ds) | Secondary Interest Impact | Total Homepage hits over unique users                        |
| 12   | ss(ds) / d(ds)  | Subset Ratio              | Subset requests over total number files downloaded           |

<br>

After extracting this data from user logs, we then calculated two index scores for a number of datasets hosted by the RDA, (including ICOADS): 

+ The **Usage Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{r}" /></a> where the given unit is (u), d is the download frequency of users, and f is the number of files downloaded per user session and n is the total number of units in the denominator, and
+ The **Interest Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(hp(u)&space;/&space;f(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" /></a> where download frequency (d) of users is replaced by the number of homepage hits (hp) a dataset receives [4](#4).

<br>

The scores that we calculated were starkly different between data products, and seemed to fluctuate grately at different times of the year. While some datasets, including ICOADS, were consistently achieving high Usage Impact Factor scores it meant relatively little from an evaluative standpoint,  unless we could compare them to other data products of a similar vein - and for many of the resources hosted by the RDA, this is impossible.  In short, our work with the DUI was unsuccessful in establishing a generic metric for calculating the impact of one resource over another. 

We then tried to typify users based on how they accessed a dataset (Weber, 2013; Weber and Thomer, 2013). Our hypothesis was that if we could develop a set of measurements for the impact that curators were having in assisting users then we might be able to make a strong economic case about the funding of this type of work. Similar work has been done in public libraries to measure the dollar value of services like a reference query \cite{jarrett2012texas}. 

In this study, the two types of users we established were:

<br>

+ **Programmatic Users**: Data is accessed or downloaded through a command line tool (e.g. '-curl [^curl] or 'wget' [^wget]) or through scripting language. 


+ **Assisted Users**: Data accessed via the graphical user interface, or by subset requests made through a separate tool developed by the RDA staff. 

<br>

What we saw emerge from the analysis of different user types were broad shifts between groups; over time programmatic users would increase, and assisted users would decrease (and vice versa). This pattern seemed to occur at very regular intervals (see figure 2 for an example from ICOADS). 

I failed to come up with a rational explanation for these patterns until talking with an ICOADS curator who explained that he would often be asked to fulfill the same subset request - not wanting to duplicate work he would write an easily modifiable script to allow an "assisted user" to download or subset records more easily.  When I went searching for evidence of these scripts in online documentation I found modified versions were abundent - posted, for instance, to a web-forumn so that anyone interested in wave swell height could access a subset of those data in ICOADS. 

This small example speaks to the difficulty in developing metrics which can quanify data use - depending on download rates, or homepage hits even through the DUI impact scores was bound to be limited in its explanation of the collaborative work that this community engaged in to overcome funding constraints. Most of the software engineers that I worked with to complete this study viewed metric based analysis skeptically - they felt it was a generic way to capture the services they provided, and as the example above showed, was complicated by their development of software to actually decrease the number of files a user had to download to get the data that they really wanted. 



 
