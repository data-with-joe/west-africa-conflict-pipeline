# west-africa-conflict-pipeline
        An end-to-end data engineering pipeline analysing organised violence and conflict trends 
        across West Africa from 1989 to 2024, built on Azure Databricks using a Medallion architecture.


## Pipeline Architecture
        Raw CSV(UCDP GED) => Bronze Layer(Raw ingestion, no transforms, Delta table) =>
        Silver Layer(Cleaned, typed, filtered, decoded, Delta table) =>
        Gold Layer(Aggregated tables powering dashboard visuals) =>
        Databricks Lakeview Dashboard


## Tech Stack

        - **Platform:** Azure Databricks (Unity Catalog)
        - **Language:** PySpark
        - **Storage Format:** Delta Lake
        - **Orchestration:** Databricks Notebooks
        - **Dashboard:** Databricks Lakeview
        - **Architecture:** Medallion (Bronze / Silver / Gold)


## Project range
        - **Coverage:** 15 West African countries, 1989–2024
        - **Raw rows:** 445,412 (global)
        - **Filtered rows:** 15,620 (West Africa)

## Key Insights
        
        - **Nigeria** recorded the highest total incidents and fatalities in West Africa,
          peaking around 2014–2015 at over 10,000 deaths in a single year, driven by 
          Boko Haram activity in the northeast.
        - **Sierra Leone** and **Liberia** dominated conflict activity in the early-to-mid 
          1990s during their respective civil wars, with near-zero activity after 2005.
        - **Burkina Faso** and **Mali** show sharp escalation from 2019 onwards, 
          reflecting the spread of jihadist insurgency across the Sahel region.
        - **One-sided violence against civilians** is the dominant violence type in Nigeria,
          highlighting the targeting of non-combatants.
        - The period **2005–2011** represents the most peaceful stretch across the region 
          in the dataset.


## Dashboard

        Built using Databricks Lakeview Dashboard, querying Gold Delta tables directly.
        
        ![Dashboard Overview](images/)


## Data Source

        This project uses data from the Uppsala Conflict Data Program (UCDP).

        - Davies, S., Pettersson, T., Sollenberg, M., & Öberg, M. (2025). Organized violence 
        1989–2024, and the challenges of identifying civilian victims. 
        Journal of Peace Research, 62(4).

        - Sundberg, Ralph and Erik Melander (2013) Introducing the UCDP Georeferenced Event 
        Dataset. Journal of Peace Research 50(4).

        - UCDP is part of and funded by DEMSCORE, national research infrastructure grant 
        2021-00162 from the Swedish Research Council.

        Data available at: https://ucdp.uu.se/downloads




