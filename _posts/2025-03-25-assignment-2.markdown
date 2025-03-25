---
layout: post
title:  "Assignment 2"
subtitle: "by Áslaug Marta (s), Ástríður María (s242976), Soffía Steingrímsdóttir (s)"
date:   2025-03-25 09:50:57 +0100
categories: jekyll update
---
*{{ page.subtitle }}*


<div class="magazine-layout">
  <!-- LEFT COLUMN -->
  <div class="column left">
    <h1>Thefted City: A Decade of Stolen Moments in San Francisco</h1>
    <p class="lede">
      A look into San Francisco's long-standing battle with theft — its spatial hotspots, shifting intensity, and the broader story behind the city’s most dominant crime.
    </p>

    <h2>Introducing the Dataset</h2>
    <p>
      This project is based on the San Francisco Police Department’s public crime reports, covering over two decades of incident data (2003–2025). The dataset includes thousands of entries with timestamps, categories (e.g. theft, assault, vandalism), and geo-coordinates. We cleaned and preprocessed the data to remove duplicates, filter out incomplete records, and exclude prostitution-related incidents (covered separately in Week 7).
    </p>

    <h2>Theft: San Francisco’s Leading Crime</h2>
    <p>
      When examining overall trends, one crime type towers over the rest: <strong>larceny/theft</strong>. With more than 725,000 reported incidents — more than triple the next highest category — theft dominates San Francisco’s crime landscape.
    </p>

    <img src="/assets/img/total_crimes.jpg" alt="Total crime occurrences by category">
    <p class="caption">Fig. 1. Total reported crime by type (2003–2025). Larceny/Theft vastly outnumbers other categories.</p>

    <p>
      Other high-frequency offenses include assault, vandalism, and vehicle theft, but none come close to the magnitude of general theft. The steep drop-off highlights just how much the city’s day-to-day crime story revolves around stolen property.
    </p>

    <h2>Where Theft Concentrates</h2>
    <p>
      The map below visualizes theft density across San Francisco using a grid heatmap. Unsurprisingly, the city’s dense commercial districts — particularly Union Square and SoMa — are where the intensity peaks.
    </p>

   <iframe src="/assets/html/theft_map.html" width="100%" height="600px" style="border:none;"></iframe>
    <p class="caption">Fig. 2. Grid-based heatmap of thefts (2003–2025), capped at 98th percentile. Darker cells indicate higher incident concentration.</p>

    <p>
      These zones are popular for shopping, tourism, and public transit — all environments where theft thrives. The map also shows spillover into nearby districts like the Mission and Tenderloin, known for socioeconomic challenges and high foot traffic.
    </p>
  </div>

  <!-- RIGHT COLUMN -->
  <div class="column right">
    <h2>Diving Into Interactivity</h2>
    <p>
      The interactive chart below lets you filter theft by time and location. This tool reveals interesting trends — like seasonal spikes during the holiday shopping season, or the drop in crime during COVID lockdowns in 2020–2021.
    </p>

<div style="width: 100%; overflow-x: auto;">
  <div style="transform: scale(0.7); transform-origin: top left; width: 680px; height: 360px;">
    <iframe 
      src="/assets/html/graf3.html" 
      style="width: 100%; height: 500px; border: none;">
    </iframe>
  </div>
  <p class="caption">Fig. 3. Yearly theft counts by district</p>
</div>

    <h2>Looking Beyond the Data</h2>
    <p>
      Several of the city’s hotspots overlap with well-known shopping corridors and high-tourism areas. Union Square, for example, has been the subject of <a href="https://www.sfchronicle.com/crime/article/union-square-theft-crime-2021-16717893.php" target="_blank">retail theft surges</a> that made headlines, especially in the post-pandemic retail recovery era.  
    </p>

    <p>
      The data also reveals how areas like the Mission District are affected by both high residential density and economic disparity — factors often linked with higher petty crime rates.
    </p>

    <h2>Final Thoughts</h2>
    <p>
      Theft isn't just a nuisance — it's the primary crime shaping the public’s experience in San Francisco. It hits residents, tourists, and businesses alike. Mapping and visualizing it at scale shows that while it’s everywhere, it’s also tightly clustered in places where opportunity meets vulnerability.
    </p>

    <h2>References</h2>
    <ul>
      <li><a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783">SF Crime Dataset (SFPD)</a></li>
      <li><a href="https://www.sfchronicle.com/crime/article/union-square-theft-crime-2021-16717893.php">SF Chronicle: Union Square Retail Theft</a></li>
      <li><a href="https://abc7news.com/sf-crime-map-data-statistics/13459019/">ABC7: SF Crime by Neighborhood</a></li>
    </ul>
  </div>
</div>