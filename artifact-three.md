---
layout: default
title: Artifact Three – Databases
nav_order: 5
---

<div style="background: rgba(255,255,255,0.035); border: 1px solid rgba(255,255,255,0.10); border-radius: 12px; padding: 24px; margin-bottom: 34px;">

<h1>Artifact Three</h1>

<h2>Database Design and Functionality</h2>

<p>This artifact focuses on improving my Grazioso Salvare dashboard application through enhancements to database design and functionality. The project was originally developed in a Jupyter Notebook for my CS-340 Client/Server Development course and connected to a MongoDB database. It included basic CRUD operations and data visualization features such as a geolocation map, data table, breed distribution chart, and rescue category filters.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Enhancement Overview</h2>

<p>I selected this project because it already included a working MongoDB connection and basic CRUD functionality, which made it a strong starting point for improving how the database handled data. The original implementation demonstrated my ability to interact with the database using PyMongo commands such as <code>find</code>, <code>insert_one</code>, <code>update</code>, and <code>delete</code>, along with basic user authentication.</p>

<p>One of the first improvements I made was replacing hardcoded user credentials with a Python-based admin authentication system that uses password hashing and access control. This allowed me to build a secure admin interface where users can create, update, and delete records, as well as manage credentials through the Dash application.</p>

<p>I then focused on improving how the database handled queries and data processing. A major enhancement was implementing MongoDB aggregation pipelines to support analytics features. I used operators such as <code>$group</code> to count outcome types, <code>$project</code> to format results into percentages, and <code>$match</code> to filter out irrelevant records. Helper functions like <code>count_outcome()</code> and <code>build_percent()</code> were used to structure this logic and prepare data for the analytics scorecards.</p>

<p>I also improved data cleaning directly within the aggregation process. Functions such as <code>build_clean_breed()</code> and <code>build_age_bucket()</code> were applied before grouping to standardize breed names and categorize animals by age. This allowed the database to return cleaner, pre-structured data that could be used directly by the application. As a result, visualizations became more consistent and easier to interpret.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Outcome Alignment</h2>

<p>This enhancement aligns with my original plan to improve database queries and shift more data processing into the database layer. By using aggregation pipelines, the system now returns structured data instead of raw records, which improves both performance and usability. These updates also support features like outcome metrics and age group analysis, showing that the application is capable of handling more advanced data processing than originally planned.</p>

<hr style="border: none; height: 1px; background: #374151; margin: 28px 0;">

<h2>Reflection</h2>

<p>This enhancement showed me how complex database logic can become when working with multiple aggregation pipelines. Early on, I noticed that the shelter.py module became difficult to manage as more logic was added. That is when I started using helper functions such as <code>build_outcome_group()</code>, <code>build_age_bucket()</code>, and <code>build_clean_breed()</code> to reduce repetition and improve readability. This made the code easier to maintain and reuse across different queries.</p>

<p>Another challenge was building aggregation pipelines in the correct order. Since each stage depends on the previous one, I had to test each step individually before combining them. This required a lot of trial and error, but it also helped me better understand how MongoDB processes data. Writing test cases for functions like <code>build_percent()</code> and <code>count_matches()</code> also helped confirm that the logic was working correctly before integrating it into the full pipeline.</p>

<p>Overall, this experience strengthened my understanding of how to structure and process data within a database. It also showed me the value of moving data processing closer to the database layer, which improves efficiency and supports more advanced analytics. These skills are directly applicable to real-world data analysis and backend development.</p>

</div>
