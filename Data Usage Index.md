###The Data Usage Index

The first of these studies was an analysis of the user logs for the Research Data Archive (RDA) where ICOADS is stored and served to end users. We hoped to develop a set of indicators based on archive - user interactions (i.e. downloads, pages visited) that would allow us to typify how ICOADS was used and consumed. To do this, we borrowed largely from an existing Data Usage Index (DUI) developed in the life sciences (). 


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

After establishing generic DUI indicators for climate related datasets (see Table 1, more details can be found in Weber et al. 2014) we calculated two index scores for ICOADS, and two similar research data products hosted by the RDA: 

+ The **Usage Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{r}" /></a> where the given unit is (u), d is the download frequency of users, and f is the number of files downloaded per user session and n is the total number of units in the denominator, and
+ The **Interest Impact Factor** <a href="http://www.codecogs.com/eqnedit.php?latex=(d(u)&space;/&space;f(u))/\sum_{1}^{n}{d}/\sum_{1}^{n}{f}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?(hp(u)&space;/&space;f(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" title="(d(u) / r(u))/\sum_{1}^{n}{hp}/\sum_{1}^{n}{f}" /></a> where download frequency (d) of users is replaced by the number of homepage hits (hp) a dataset receives [4](#4).

In short, our work with the DUI was unsuccessful in establishing a generic metric for calculating the impact of one resource over another. In  attempt to extend this work, we tried to typify users based on how they accessed a dataset (Weber, 2013; Weber and Thomer, 2013). The two types of users we established were:

1. **Programmatic Users**: Data is accessed or downloaded through a command line tool (e.g. '-curl [^curl] or 'wget' [^wget], and 

2. **Assisted Users**: Data accessed via the graphical user interface, or submitted subset requests through a separate tool developed by the RDA staff. 

While this work also failed to establish a generic set of data usage metrics, what we saw emerge from the analysis of different user types were broad shifts between groups; over time programmatic users would increase, and assisted users would decrease (and vice versa), and whats more this often happened at very regular intervals (see figure 2 for an example from ICOADS). 

I failed to come up with a rational explanation for these patterns until talking with an ICOADS curator who explained that occasionally he would fulfill the same subsetting request too many times, and would be motivated to write a new script that would allow an "assisted user" to download or subset records very easily - he could point to dates when that occurred, and the rise of programmatic users, versus new releases of ICOADS - and the subsequent breaking of a script and the rise of assisted users. While this seems like a trite example on its face, it speaks to how complicated constructing metrics are for 

 