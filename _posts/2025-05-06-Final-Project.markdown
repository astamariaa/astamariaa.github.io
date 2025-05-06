---
layout: post
title:  "Assignment 2"
subtitle: "by Áslaug Marta (s232721), Ástríður María (s242976), Soffía Steingrímsdóttir (s242691)"
date:   2025-05-06 09:50:57 +0100
categories: jekyll update
---
*{{ page.subtitle }}*


<div class="magazine-layout">
  <!-- LEFT COLUMN -->
  <div class="column left">
    <h1>San Francisco Crime data 2003-2025.</h1>
    <p class="lede">
      In this workbook the crime data from 2003 to 2025 will be examined. The crime that will be focused on and explored is Larceny/Theft. 
    </p>

    <h2>Introduction to the dataset</h2>
    <p>
      This project utilizes the San Francisco Police Department's publicly available crime reports, covering over two decades of incident data (2003–2025).  The data set includes thousands of records with  timestamps, categories ( theft, assault, vandalism etc.), and geo-coordinates. We preprocessed and cleaned the data for duplicate removal,  removal of incomplete records and discarded other irrelevant columns. 
    </p>

    <h2>San Francisco’s Leading Crime: Larceny/Theft</h2>
    <p>
      When looking through the dataset and its overall trends, one crime type clearly stands out as more common than the rest: Larceny/Theft. There are over 725,000 reported incidents, which is more than three times higher than the second most reported crime. 
      
      As seen in Figure 1, other crimes like Assault, Vandalism, and Vehicle Theft also appear often, but even when combined, they don’t reach the same numbers as Larceny/Theft. Because of how common it is and how much it stands out from the rest, Larceny/Theft was chosen as the most interesting crime type to look further into in this assignment.
    </p>

    <img src="/assets/img/total_crimes.jpg" alt="Total crime occurrences by category">
    <p class="caption">Fig. 1. Total reported crime by type (2003–2025). Larceny/Theft vastly outnumbers other categories.</p>

    <h2>Where do these crimes happen?</h2>
    <p>
     Figure 2 presents a grid-based heatmap of Larceny/Theft incidents reported between 2003 and 2025. Each square represents one square kilometer. Darker colors show  areas where more incidents have been reported, and the data is capped at the 98th percentile to prevent extreme values from skewing the view. Most Larceny/Thefts are concentrated in and around downtown San Francisco. A few central grid cells stand out as the darkest, meaning those areas consistently had the highest number of theft reports over the twenty-year period. These zones are popular for shopping, tourism, and public transit — all environments where theft thrives. Moving outward from the city center, the number of incidents drops off,  shown by the lighter-colored squares. By clicking the boxes, you can see the exact number of thefts happening in that area. 
    </p>

   <iframe src="/assets/html/theft_map.html" width="100%" height="600px" style="border:none;"></iframe>
    <p class="caption">Fig. 2. Grid-based heatmap of thefts (2003–2025), capped at 98th percentile. Darker cells indicate higher incident concentration.</p>
 
 </div>

  <!-- RIGHT COLUMN -->
  <div class="column right">

    <h2>Interactive Visualization </h2>
    <p>
      The interactive chart below shows yearly Larceny/Theft data in different areas from 2003 to 2025. It allows the user to select which areas to display - it can be one, a couple or all of them. Southern district consistently shows the highest theft counts across almost all years. The northern and central district also show high crimerates, likely due to the fact that those are some tourist areas. The lower theft areas such as Ingleside, Park and Richmond are probably due to the fact that those are more residential areas. This chart also presents interesting trends - like the drop in crime in 2020-2021 which could most likely be due to the COVID lockdowns. Theft also increased after 2011 which could possibly be due to changes in policing strategy.
    </p>

 <div style="width: 100%; overflow-x: auto;">
  <div style="transform: scale(0.7); transform-origin: top left; width: 500px; height: 360px;">
    <iframe 
      src="/assets/html/graf3.html" 
      style="width: 100%; height: 500px; border: none;"
      >
    </iframe>
  </div>
  <p class="caption">Fig. 3. Yearly Larceny/Theft incidents by district (2003–2025), with higher rates in tourist areas and a drop during 2020–2021 due to COVID-19.</p>
</div>

    <h2>Looking beyond the data</h2>
    <p>
      Some of the city’s biggest theft hotspots line up with popular shopping areas and tourist spots. Take Union Square, for example, there are waves of retail theft, especially during the post-pandemic recovery when a lot of stores were just trying to get back on their feet. The Mission District stands out too, it’s a mixed neighborhood dealing with big income gaps, which often goes hand-in-hand with petty theft. It’s a reminder that theft isn’t just about opportunity, it’s also tied to economic positions.
    </p>



    <h2>Final thoughts</h2>
    <p>
      In conclusion, this project highlights how Larceny/Theft has shaped San Francisco’s crime landscape over the past two decades. By combining time-based trends, geographic heatmaps, and interactive tools, we can see how theft patterns reflect the city’s social and economic realities - from retail-heavy downtown zones to residential neighborhoods. The impact of events like the pandemic is clear in the data, as are  shifts tied to policy and urban change. Understanding when and where these crimes happen gives us valuable insight into how cities function — and where there’s room for smarter, more responsive public safety strategies.
    </p>

    <h2>Contribution</h2>
    <p>
      All team members contributed equally to the project. Ástríður set up the website, the websites design and created Charts 1 and 2. Soffía was responsible for Chart 3 and contributed to the data analysis and writing. Áslaug led most of the analytical work and wrote the majority of the text for the final report.
    </p>
  </div>
</div>