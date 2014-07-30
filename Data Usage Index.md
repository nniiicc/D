###The Data Usage Index

The first of these studies was an analysis of user logs from the Research Data Archive (RDA) where ICOADS is hosted and served to end users. In this work, we hoped to develop a set of indicators based on data access events (e.g. downloads, pages visited, etc.) that would allow us to make a more robust set of statements about ICOADS impact than simply saying how many times it had been downloaded. To do this, we borrowed largely from an existing Data Usage Index (DUI) developed in the life sciences \cite{chavan2009towards,ingwersen2011indicators}. In adapting the DUI for climate related data products we first developed a suite of DUI indicators specific to the types of interaction events that were appropriate for RDA users (see Table 1, more details can be found in Weber et al. 2013).

After extracting this data from the RDA's user logs, we then calculated two index scores for datasets hosted by the RDA, (including ICOADS): 

+ The **Usage Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{r}" /></a> where (u) is the given resource unit, d is the download frequency of users, f is the number of files downloaded per user session, and n is the total number of units in the denominator, and
+ The **Interest Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(hp(u)&space;/&space;f(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" /></a> which is identical to UIF except download frequency (d) of users is replaced by the number of homepage hits (hp) a dataset receives [4](#4).

<br>

The scores that we calculated were starkly different between data products, and seemed to fluctuate greatly at different times of the year. While some datasets, including ICOADS, were consistently achieving high Usage Impact Factor scores there seemed no universal explanation for how fluctuations should be interpreted, and in what context these scores would be useful for making reliable statements about the impact of a resource.  In short, our work with the DUI was unsuccessful in establishing a generic metric for calculating impact based on data access. 

In this study, we also tried to typify users based on _how_ they accessed a dataset (Weber, 2013; Weber and Thomer, 2013). Our hypothesis was that if we could develop a set of measurements for the impact that curators were having in assisting users then we might be able to make a strong economic case about the funding of this type of work. Similar work has been done in public libraries to measure the dollar value of services like a reference query \cite{jarrett2012texas}. 

In this study, the two types of users we established were:

<br>

+ **Programmatic Users**: Data is accessed or downloaded through a command line tool (e.g. '-curl [^curl] or 'wget' [^wget]) or through a scripting language. 


+ **Assisted Users**: Data accessed via the graphical user interface, or by subset requests made through a separate tool developed by the RDA staff. 

<br>

What we saw emerge from the analysis of different user types were broad shifts between groups; over time programmatic users would increase, and assisted users would decrease. This pattern seemed to occur at very regular intervals (see figure 2 for an example from ICOADS). 

We failed to come up with a rational explanation for these patterns until talking with an ICOADS curator who explained that he would often be asked to fulfill the same subset request, and not wanting to duplicate work he would write an easily modifiable script to allow a user to download or subset records more easily - essentially converting an "assisted user" to a "programmatic user." And this transformation had a cascascading effect; when I went searching for evidence of these scripts in online documentation I found modified versions were abundant, being posted, for instance, to a web-forum so that anyone interested in wave swell height could access a subset of those data in ICOADS. 

This small example speaks to the difficulty in developing metrics which can quantify data use - depending on download rates, or homepage hits even through the DUI impact scores was bound to be limited in its explanation of the collaborative work that this community engaged in to overcome funding constraints. In economic terms, what we were missing with these metrics were transaction costs \cite{williamson1989transaction}, for example learning how to download data, negotiating subsets of the data, and agreeing upon (contractually) how data were to be organized and served, etc. What the curators were doing, in terms of lowering transaction costs for end-users, was to provide a positive spillover or an externality that resulted in a net-economic gain, but an immediate or calcuable loss in terms of the metrics we had created. Callon's work on the intersection of sociology and economics has demonstrated that even outside the "marketplace" model of organizing, positive spillovers remain a salient concept for understanding work place motivations, and explaining what seems to be irrational actors \cite{callon1998essay}. The task of undersanding ICOADS sustainbility in terms of these types of net, or total community gains remained a salient and open question, and one that would require different approaches than metric based analysis of usage impact. 
