# K-Means Clustering Analysis of Asthma Related Deaths and Fuel Type in the Bay Area

By Mihir Thakar

This Project is going to correlate Vehicle and Health data from 9 counties that make up the Bay Area. I obtained an "Asthma Deaths by County" and "Vehicle Fuel Type by Zip Code" dataset from the CA.gov open data portal. The most important task will involve organizing the zipcoded data into an organized data frame as each county is host to multiple zip codes. From there I will be able to connect whether the fuel type (Hybrid, Elec, Gas) has an affect on the presence of Asthma deaths and create a visualization based on most K-Means Clustering. The final results are then geocoded into chloropleth maps. You can follow my work pipeline below.

First off I cleaned the 2 Datasets.

Here is an example of the cleaned Asthma Dataset according to the counties

<img src="Images/image_2022-05-04_193008617.png" alt="Image description">
{:style="display:block; margin-left:auto; margin-right:auto"; :height="75%" width="75%"; }
{:refdef: style="text-align: center;"}
*Asthma Frame*
{: refdef}


Here is an example of the cleaned FuelType Dataset according to the zipcode

<img src="Images/CleanFuel.png" alt="Image description">
{:style="display:block; margin-left:auto; margin-right:auto"; :height="75%" width="75%"; }
{:refdef: style="text-align: center;"}
*Fuel Type Frame*
{: refdef}

By creating a dictionary of zipcodes for each County I was able to map each zipcode to the 9 counties of the Bay Area.
I then used a groupby method to find the number of Deaths in each county

<img src="Images/AnalysisFrame.png" alt="Image description">
{:style="display:block; margin-left:auto; margin-right:auto"; :height="75%" width="75%"; }
{:refdef: style="text-align: center;"}
*Death GroupBy Frame*
{: refdef}


The Final results ultimately cleaned the code to analyze only the 9 Bay Area counties to make the following Final Frame

<img src="Images/FinalFrame.png" alt="Image description">
{:style="display:block; margin-left:auto; margin-right:auto"; :height="75%" width="75%"; }
{:refdef: style="text-align: center;"}
*Final Frame*
{: refdef}



<iframe src="Maps/DP.html" height="500" width="500"></iframe>


<iframe src="Maps/AV.html" height="500" width="500"></iframe>


<iframe src="Maps/AC.html" height="500" width="500"></iframe>
