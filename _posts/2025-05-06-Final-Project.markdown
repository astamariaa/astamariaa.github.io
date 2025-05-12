---
layout: post
title:  "From Kickoff to Final Whistle: Exploring Factors Influencing Stadium Attendance"
subtitle: " 02806 Social Data Analysis and Visualization - Project Assignment B: The Viz and the Notebook. Workbook by Áslaug Marta (s232721), Ástríður María (s242976) and Soffía Steingrímsdóttir (s242691)"
date:   2025-05-06 09:50:57 +0100
categories: jekyll update
---
*{{ page.subtitle }}*


<div class="magazine-layout">
  <!-- LEFT COLUMN -->
  <div class="column left">
    <h1>Premier League data 2019-2024.</h1>
    <p class="lede">
      In this workbook, we will dive into the data of the past five seasons of the English Premier League through the lens of social data analytics. 
We chose this topic due to the fact that we are all big football fanatics, and therefore it is intriguing to examine some interesting factors of the Premier League. 
We want to explore football attendance to help us get an understanding of the impact of fan engagement, assess stadium utilization, the timing of the games and potentially predict and help with stadium planning. Subsequently, we’ll conduct a thorough investigation to find the underlying reasons behind the patterns we uncover. 
    </p>

  <h2>Introduction</h2>
    <p>
    Football culture plays immense value on the presence of fans in the stadium. They say that crowds can have a sway over the results of the game, put pressure on the referees and intimidate opponents.  But does this hold true in the real world? We want to examine whether the data reflects this romanticized idea of fans' attendance at football games and their influence on the match.  In this notebook, the connection between match attendance and team performance will be explored, and a specific focus on home matches in the English Premier League across five seasons (2019/2020 to 2023/2024). The goal is to quantify trends in attendance and evaluate whether a fuller stadium correlates with better home performance.  On top of that we want to assess stadium utilization, the timing of the games and potentially predict and help with stadium planning. Subsequently, we’ll conduct a thorough investigation to find the underlying reasons behind the patterns we uncover.
    </p>

  <h2>The teams</h2>
    <p>
    There are 20 teams in the Premier League. Each year, the bottom three teams of the league are relegated while three teams are promoted to take their place. For the past 5 seasons, 28 teams have played in the league.  Some teams like Liverpool, Manchester City and Manchester United have remained consistent participants in the Premier League, while others like Fulham and West Brom have moved in and out of the league. This turnover adds variety to the league and introduces differences between seasons in things like stadium capacities, fan culture and team performance dynamics. 

  </p>


  <h2>Average Attendance</h2>
    <p>
    The most logical thing is to start our analysis on the data was to begin with examining the stadiums of the teams. We began with comparing the average attendance of all games in the league by seasons. It is clear to see that obviously the Covid-19 pandemic restrictions affected the attendance to the games significantly. However it is interesting to see that after the pandemic, attendance has increased by approximately 10.000 persons per game, peaking in 2023. 
    </p>

  <img src="/assets/img/mynd1.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
  <p class="caption"><strong>Fig. 1:</strong> Average attendance per Premier League season from 2018 to 2024.</p>
 
 <h2>Average stadium attendance vs average stadium fill percentage</h2>
    <p>
      Next up we thought it could be interesting to take a look at the attendance of the games.  We decided to compare the average stadium attendance vs the average stadium fill percentage. It was no surprise to see that there are mostly just the largest clubs in the league that appear  in the top 10 the highest stadium fill, with Manchester United at the top, with average attendance over 50.000. However it was quite interesting to see that if we look at the average stadium fill percentage, the Manchester United only fills their stadium about 75% on average. Eight out of the top ten clubs are considered relatively small, with Brentford at the top with on average 98.7% stadium fill at their games. Of course many of these clubs have smaller stadiums which are easier to fill, for example the capacity at Brentfords home stadium is approx 17.000 seats, but this reflects a loyal local fanbase to the smaller clubs which are outperforming the larger ones with efficiency. The high average attendance mostly reflects on the clubs size but the high fill percentage reflects on fan enthusiasm and sell-out consistency.  Here you can also see a heatmap of the where the stadiums are marked as dots. By clicking the dots, you are able to see the stadium name along with the average stadium fill percentage. 
    </p>

  <img src="/assets/img/mynd2.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
  <p class="caption"><strong>Fig. 2:</strong> Top 10 Stadiums by Average Attendance.</p>

  <img src="/assets/img/mynd3.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 3:</strong> Average Stadium Fill Percentage by Club.</p>

  <iframe src="/assets/html/england_stadium_fill_map.html" width="100%" height="600px" style="border:none;"></iframe>
  <p class="caption"><strong>Fig. 4:</strong> Interactive map showing average stadium fill percentage.</p>


  <h2>Timing of games - attendance by time and day</h2>
    <p>
     We then examined the timing of the games - and if there were any noticeable patterns between the attendance of the games and the timing.  From the heatmap you can see that Thursday games at 17:30 have the highest attendance, with about 70.000 people. That however is likely based on fewer matches as Thursday fixtures are rare and mostly for special events like European reschedules. However Sundays have the highest overall attendance both for the 15:30 and 17:30 slots. The attendance is consistently high and the games at this time are frequent, making it the most reliably strong day overall attendance vice.
    </p>

  <img src="/assets/img/mynd4.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 5:</strong> Heatmap showing average attendance by kickoff time and weekday.
.</p>

<p>
Here you can see a map of all the stadiums color coordinated by the most common timing of their games. 
 </p>

   <iframe src="/assets/html/mtime" width="100%" height="600px" style="border:none;"></iframe>
<p class="caption"><strong>Fig. 6:</strong> Map showing each stadium’s most common kickoff time.</p>


 </div>

  <!-- RIGHT COLUMN -->
  <div class="column right">


 <div style="width: 100%; overflow-x: auto;">   
</div>


  <h2>3pm blackout</h2>
  <p>
     The 3pm blackout was established in the 1960’s UK football and refers to a long-standing rule that no football matches in any league can be broadcasted live on TV in the UK between 2:45pm and 5:15pm on Saturdays. The reason behind this rule was due to the fact that it was feared that televised top-tier games, such as Premier League games,  would reduce attendance to local teams in lower leagues if fans stayed home to watch on TV instead.  We decided to examin the games that are during this blackout period further.  It is clear to see that the attendance of the games during the blackout is significantly better then to the other games as you can see on this simple bar graph. 
  </p>

  <img src="/assets/img/mynd6.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 7:</strong> Average stadium fill rate comparison: 3PM Saturday vs. other matches.
</p>
  
<p>
    From the chart here down below you can see that the smaller clubs play more often during the blackout period, this is likely due to the fact that those games are moved to the traditional kickoff time at 3pm on Saturdays since they have lower media prioritization and less broadcast demand. 
Then it of course makes sense that the teams that are the least affected by the blackout are the biggest clubs in the league, as their matches are frequently picked for live broadcast due to large followings and high viewership demand.
</p>

  <img src="/assets/img/mynd7.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 8:</strong> Club-level breakdown of how often each team plays during the 3PM blackout window.
</p>

<p>
If we take a look at the number of matches played per month, interesting data is gathered. On first look we can see that December is the busiest month almost each season. English football uniquely embraces a packed schedule over the holidays since the holiday period  equals high TV viewership and stadium attendance.
If we examine the data further, we see that relatively few games were played in September 2022 compared to the other years, which could be due to the fact that Queen Elizabeth II passed away in September that year, and therefore, a few games were postponed. That happened both the following days after she passed away and the day of her funeral.
There were also more games played in August and October that season, likely due to the fact that the World Cup was held in November and December that year. Therefore some of  the games had to be shifted to earlier. 
</p>

  <img src="/assets/img/mynd8.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 9:</strong> Number of matches played per month (August–January) across seasons.
</p>



 <h2>Results of the games</h2>
    <p>
      From this graph we can see that Manchester United has the overall most wins, both at home and away. At the same time do  West Brom, Luton, and Norwich have the fewest wins overall.  We were debating if indeed it mattered for the team's performance if the game was played at their home stadium or away. It is clear from the graph that it does in fact matter, since all the teams perform better at their home games than away. This show how important it is to the clubs to have a strong fan base. Clubs like Brentford, Crystal Palace, and West Ham show noticeable home-away gaps, suggesting a strong home advantage and rely heavily on their fans. 
    </p>

 <p>
    On the heatmap below you can find all the stadiums and the the ratio between home, away and draws on that stadium. 
 </p>

   <iframe src="/assets/html/mynd9.html" width="100%" height="600px" style="border:none;"></iframe>
<p class="caption"><strong>Fig. 10:</strong> London stadiums colored by home win percentage (with W/D/L tooltips).
.</p>



 <h2>Does higher xG attract more attendance?</h2>
    <p>
      As average home xG increases, average attendance generally rises. Fans are more likely to show up for teams that create more chances. However, the relationship between those two variables is not necessarily causal.  Bigger crowds may correlate with stronger clubs that naturally have higher xG due to having more money and therefore better players.
Then there are the outliers, for example Manchester United and Westham that have lower xG’s but still attract big crowds, due to big club royalty among the fans. 
    </p>

  <img src="/assets/img/mynd10.png" alt="Average Attendance Plot" style="width:100%; max-width:800px;">
<p class="caption"><strong>Fig. 11:</strong> Correlation between average xG and average home attendance.
</p>

  <h2>Final thoughts</h2>
    <p>
      Through this comprehensive analysis of Premier League data, we gained valuable insights into the relationships between team performance, fan engagement, and scheduling dynamics. One of the most consistent patterns was the significant advantage of playing at home, with nearly all clubs showing notably higher home win counts than away. This proves the importance of the fans' support for the teams. 
We also discovered that stadium attendance and fill rates don’t always align with on-pitch success, that sunday afternoon fixtures are the most popular amongst the fans and that the 3 pm blackout does in fact enhance the stadium attendance. 
The correlation between xG and attendance showed that fans are indeed drawn to exciting, high scoring teams, but at the same time do teams with long history, tradition, and large stadium capacity often override pure performance.
Overall, this analysis has deepened our interest in the Premier League. It highlights how both on-field success and off-field factors shape the world of modern football.

   </p>

  <h2>Contribution</h2>
    <p>
      BLA
    </p>
  </div>
</div>