---
layout: default
title: Artifact Two – Algorithms & Data Structures
nav_order: 4
---

<div style="background: rgba(255,255,255,0.035); border: 1px solid rgba(255,255,255,0.10); border-radius: 12px; padding: 24px; margin-bottom: 34px;">

<h1>Artifact Two</h1>

<h2>Algorithms and Data Structures</h2>

<p>This artifact focuses on improving my Grazioso Salvare dashboard application through the use of algorithms and data structures. The project was originally developed in a Jupyter Notebook for my CS-340 Client/Server Development course. For this enhancement, I continued working with the same application and focused on improving how the data is processed and structured to support more meaningful analysis.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Enhancement Overview</h2>

<p>In the original version of the application, data processing was fairly simple. The system relied on basic CRUD operations, along with looping through records and applying conditional logic based on user-selected filters. When a rescue category was selected, the application would iterate through the dataset, return matching records, and update the table, chart, and map. While this approach worked, it was limited to basic filtering and did not support deeper analysis.</p>

<p>To improve this, I focused on restructuring how the data was processed using grouping, categorization, and transformation techniques. For example, I used pandas functions such as <code>pd.to_datetime()</code> to convert date fields, then applied <code>groupby()</code> and <code>pivot()</code> to create trend-based visualizations. This allowed me to build charts that show how outcomes change over time, making patterns in the data easier to identify.</p>

<p>I also implemented more advanced data structures to support visualizations like the breed outcome sunburst chart. This required grouping data by fields such as <code>animal_group</code> and <code>outcome_group</code>, then restructuring the results into a parent-child format so the chart could display relationships between categories. Additional improvements included calculating outcome percentages for summary metrics and grouping animals into age categories to support clearer visualizations. These changes allowed the application to move beyond simple filtering and instead provide meaningful analytical insights.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Outcome Alignment</h2>

<p>This enhancement aligns with my original plan to expand beyond basic data filtering and focus more on how data is processed and structured. By applying grouping, categorization, and transformation techniques, I was able to improve the analytical capabilities of the application. These updates allowed the system to support more advanced visualizations and provide more value to the user, without changing the overall direction of my original plan.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Reflection</h2>

<p>This enhancement helped me better understand how important data structures and algorithms are when working with real datasets. It became clear that meaningful visualizations depend heavily on how the data is prepared and structured beforehand. Applying feature engineering techniques, such as creating grouped fields and transforming date values, made a significant difference in how the data could be analyzed.</p>

<p>One challenge I ran into was working within the limitations of the dataset. For example, I initially wanted to build a chart showing how long animals stayed in the shelter, but the dataset did not include intake datetime data, so that was not possible. Another challenge was building the sunburst chart, since I had to restructure grouped data into a parent-child hierarchy, which was something I had not worked with before. This required additional processing to organize the data into a format that the visualization could use.</p>

<p>Overall, this experience showed me how to take raw data, work through its limitations, and transform it into something that supports meaningful analysis. These are skills that directly apply to real-world data analysis and development work.</p>

</div>
