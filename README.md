Download Link: https://assignmentchef.com/product/solved-csye7245-lab5-snowflake
<br>
This lab demonstrates working with Snowflake data cloud, querying, data loading, caching, cloning, user roles and permissions and time travel concepts.

Snowflake’s Data Cloud is powered by an advanced data platform provided as Software-as-a-Service (SaaS). Snowflake enables data storage, processing, and analytic solutions that are faster, easier to use, and far more flexible than traditional offerings.Snowflake combines a completely new SQL query engine with an innovative architecture natively designed for the cloud. To the user, Snowflake provides all of the functionality of an enterprise analytic database, along with many additional special features and unique capabilities.




Snowflake is a true SaaS offering. More specifically:

<ul>

 <li>There is no hardware (virtual or physical) to select, install, configure, or manage.</li>

 <li>There is virtually no software to install, configure, or manage.</li>

 <li>Ongoing maintenance, management, upgrades, and tuning are handled by Snowflake.</li>

</ul>

Snowflake runs completely on cloud infrastructure. All components of Snowflake’s service (other than optional command line clients, drivers, and connectors), run in public cloud infrastructures.

Snowflake’s architecture is a hybrid of traditional shared-disk and shared-nothing database architectures. Similar to shared-disk architectures, Snowflake uses a central data repository for persisted data that is accessible from all compute nodes in the platform. But similar to shared-nothing architectures, Snowflake processes queries using MPP (massively parallel processing) compute clusters where each node in the cluster stores a portion of the entire data set locally. This approach offers the data management simplicity of a shared-disk architecture, but with the performance and scale-out benefits of a shared-nothing architecture.

<h1><strong>Dataset:</strong></h1>

We used 2  data sets in our lab one was trips and the other was weather and it was staged on Snowflake from S3 bucket.

s3://snowflake-workshop-lab/citibike-trips

s3://snowflake-workshop-lab/weather-nyc




<h1><strong>Experiment setup:</strong></h1>

To Prepare for our Lab Environment we registered for a <a href="https://trial.snowflake.com/">Snowflake free 30-day trial</a> and used Snowflake Enterprise Edition, AWS cloud provider, and selected US East region. After registering, we received an email with an activation link of our Snowflake account URL

<h1><strong>Test Cases</strong></h1>

<h2><strong>Preparing to Load Data</strong></h2>

We performed below steps in this section:

<ul>

 <li>created a database and table</li>

 <li>created an external stage</li>

 <li>created a file format for the data</li>

</ul>



















Databases

Roles




























Table

Stages







<h2>Loading Data</h2>

<ul>

 <li>Created new Warehouse</li>

 <li>Loaded data into table</li>

</ul>













<h1><strong>Results</strong></h1>

<h2>Analytical Queries, Results Cache, Cloning</h2>




<ul>

 <li>Executing SELECT Statements and Result Cache</li>

</ul>































Caching:






















Cloning:

<h2>Working With Semi-Structured Data, Views, JOIN</h2>

<ul>

 <li>Loaded weather data in JSON format held in a public S3 bucket</li>

 <li>Created a View and query the semi-structured data using SQL dot notation</li>

</ul>

Json data






















Creating view

Joining trips data and weather view

<h2></h2>

<h2></h2>

<h2>Time Travelling</h2>

Restoring weather table after dropping it accidentally




Updating the records with wrong data and then rolling back the action

<h2>Role based Access Controls</h2>




Preview

<h1>Lessons learned</h1>







<ol>

 <li>Learned to create stages, databases, tables, views, and warehouses on Snowflake</li>

 <li>Learned to load structured and semi structured data, querying the tables and cloning the table</li>

 <li>Also learned to grant privileges to roles and time travelling i.e rolling back the dropped table  and updated records.</li>

</ol>




References

<a href="https://guides.snowflake.com/guide/getting_started_with_snowflake/#11">https://guides.snowflake.com/guide/getting_started_with_snowflake/#11</a>












































