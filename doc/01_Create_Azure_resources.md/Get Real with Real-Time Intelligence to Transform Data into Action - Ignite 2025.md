---
title: 'Get Real with Real-Time Intelligence to Transform Data into Action - Ignite 2025'
layout: default
nav_order: 26
parent: 'Lab summaries'
---

**ID** 205272
**Number:** LAB532
**Name:** Get Real with Real-Time Intelligence to Transform Data into Action - Ignite 2025
**CloudSubscriptionPoolName:** Ignite 2025 - CSS
**AllowSave:** False
**CloudCredentialPoolAssignments:** NA
**Additional licenses:** NA

---

### Exercise Summary

**Exercise 1: Create Resources**
	- **Goal:** Set up the foundational environment in Microsoft Fabric for real-time intelligence.
	- **Actions:**
		- Sign in to Microsoft Fabric portal and create a new workspace with Fabric Capacity.
		- Create an Eventhouse, which also provisions a KQL database.
	- **Validation:** Workspace and Eventhouse are visible in the portal with correct configuration.

**Exercise 2: Get Data in the Real-Time Hub**
	- **Goal:** Ingest and transform streaming data using the Real-Time hub.
	- **Actions:**
		- Create an eventstream and connect to the sample "Bicycle rentals" data source.
		- Add a timestamp transformation to incoming events.
		- Configure a destination Eventhouse and KQL database table for the transformed data.
		- Activate and publish the eventstream pipeline.
	- **Validation:** Data flows into the RawData table in the KQL database; eventstream is active and error-free.

**Exercise 3: Set an Alert on Your Event Stream**
	- **Goal:** Monitor streaming data and receive notifications for critical conditions.
	- **Actions:**
		- Set up an alert rule on the eventstream to trigger when the number of bikes falls below a threshold.
		- Configure alert actions to send notifications and save alert details.
	- **Validation:** Alert rule is created and visible; test by simulating or observing a low bike count event.

**Exercise 4: Transform Data in a KQL Database**
	- **Goal:** Organize and transform ingested data using KQL and update policies.
	- **Actions:**
		- Move the RawData table to a Bronze folder using KQL.
		- Create a Silver-layer TransformedData table with an enhanced schema.
		- Develop a KQL function for data transformation and apply it via an update policy.
		- Verify transformation by comparing source and target tables.
	- **Validation:** TransformedData table contains processed records with expected schema and values.

**Exercise 5: Query Streaming Data Using KQL**
	- **Goal:** Analyze and visualize real-time data using KQL queries and materialized views.
	- **Actions:**
		- Write KQL queries to filter and visualize data (e.g., time charts for bike availability).
		- Create a materialized view for aggregated, up-to-date results.
		- Query using T-SQL and convert SQL to KQL.
		- Use Copilot to generate KQL queries from natural language prompts.
	- **Validation:** Visualizations and query results display correct, real-time data; materialized view is accessible.

**Exercise 6: Create a Real-Time Dashboard**
	- **Goal:** Build interactive dashboards to monitor and explore real-time data.
	- **Actions:**
		- Pin KQL query results as tiles to a new Real-Time dashboard.
		- Add and configure additional visual tiles (e.g., maps, charts) using query outputs.
		- Edit and format dashboard tiles for clarity.
	- **Validation:** Dashboard displays live data visualizations; tiles update as data changes.

**Exercise 7: Create Anomaly Detection on Your Data**
	- **Goal:** Detect and alert on unusual patterns in streaming data.
	- **Actions:**
		- Configure anomaly detection on the TransformedData table.
		- Select attributes and run analysis to identify anomalies.
		- Create and configure alert rules for detected anomalies, including notification actions.
	- **Validation:** Anomalies are detected and displayed; alerts are triggered and delivered as configured.

**Exercise 8: Create Map**
	- **Goal:** Visualize geospatial data using maps in Microsoft Fabric.
	- **Actions:**
		- Create a KQL queryset for map visualization.
		- Set up a Lakehouse and upload GeoJSON files for geographic context.
		- Create a Map item, add eventhouse and Lakehouse data layers, and configure map visuals (e.g., tooltips, series groups).
	- **Validation:** Map displays bike station data and geographic layers; interactive features function as expected.

**Exercise 9: Use Data Agent on Your Data**
	- **Goal:** Enable natural language querying and insights on real-time data using a Data Agent.
	- **Actions:**
		- Create a Data Agent and connect it to the eventhouse data source.
		- Provide agent instructions for data analysis.
		- Interact with the agent using natural language questions about bike availability and trends.
	- **Validation:** Agent responds accurately to queries; insights reflect current data.

**Exercise 10: Clean Up Resources**
	- **Goal:** Remove all lab-created resources to avoid unnecessary usage or charges.
	- **Actions:**
		- Delete individual items (eventstream, eventhouse, KQL queryset, dashboard, map, data agent) or the entire workspace.
	- **Validation:** Workspace and all associated resources are deleted and no longer visible in the portal.