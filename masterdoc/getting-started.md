# Real Time Analytics with Synapse

### Overall Estimated Duration: 4 Hours

## Overview

This interactive lab begins with exploring an integrated Data Lakehouse foundation, focusing on data ingestion, transformation, and analytics using ADX, Synapse, Azure Databricks, and Microsoft Purview. It includes exercises for creating pipelines, combining data, and investigating ML and Power BI scenarios. 

## Objective

Understand how to unify data estates using the Microsoft Intelligent Data Platform and manage a Data Lakehouse. Learn data ingestion, transformation, and reporting for accelerated value creation. By the end of this lab, you will have knowledge on :

### Analytics in the Microsoft Intelligent Data Platform Lab

- **Data ingestion from a spectrum of analytical and operational data sources into the Lakehouse** : Learn to implement data ingestion pipelines using ADX for streaming data and Synapse pipelines to ingest raw data from analytical and operational sources into the Bronze layer of the Data Lake.
- **Explore offline data and analytics pipeline using open Delta format and Azure Databricks Delta Live Tables. Stitch streaming and non-streaming data (landed earlier) to create a combined data product to build a simple Lakehouse** : Learn to use the open Delta format and Azure Databricks Delta Live Tables for offline data and analytics pipelines.
- **Explore Machine Learning and Business Intelligence scenarios on the Lakehouse** : Learn to explore ML and BI scenarios on the Lakehouse using Azure Databricks MLflow, Power BI, and SQL Analytics with Azure Synapse Serverless and Databricks.
- **Glimpse of Purview to govern the overall data and analytics estate.** : Explore the wide range of possibilities — including data discovery and classification, end-to-end lineage, a centralized data catalog, policy and access control enforcement, and integration to ensure compliant, discoverable, and well-governed analytics across your estate.

## Pre-requisites

- **Basic Understanding of Data Architecture**: Familiarity with data lakehouse and data warehouse concepts.

## Architecture

In this lab, the architecture covers two main aspects: first, it explores an integrated Data Lakehouse foundation using ADX, Synapse, and Azure Databricks for efficient data ingestion, transformation, and analytics, supporting ML and BI scenarios with governance by Microsoft Purview. Secondly, it delves into building and managing a unified data lakehouse, which includes creating a workspace, ingesting and preparing data, and leveraging Delta Lake for streamlined data processing and reporting through tools like Power BI.

## Architecture Diagram

![](../media/arch-new.png)

## Explanation of Components

- **Azure Synapse Analytics** : Integrates data ingestion and transformation with serverless SQL and data pipelines, enabling seamless preparation and analysis of large datasets.
- **Azure Databricks** : Facilitates advanced data transformation and machine learning with Delta Live Tables and SQL analytics, optimizing data workflows and model training.
- **Microsoft Purview** : Ensures comprehensive data governance and cataloging, providing a unified view and management of the entire data estate.
- **Power BI** : Enables interactive data visualization and reporting, allowing users to derive actionable insights from the data lakehouse.
- **Delta Lake** : Standardizes data storage with a unified format that supports reliable and scalable data processing across various analytics tools.
- **Lakehouse** : Combines the best features of data lakes and data warehouses, offering a unified data platform that supports both structured and unstructured data for comprehensive analytics, machine learning, and business intelligence.
- **Notebooks** : Provide an interactive environment for data exploration and analysis, allowing users to perform ad-hoc queries and visualize results using code or SQL.
- **Dataflows** : Enable the design and automation of data transformation processes within a visual interface, simplifying the ETL (Extract, Transform, Load) workflows.
- **Pipelines** : Orchestrate and automate data ingestion and processing tasks, integrating various data sources and ensuring smooth data movement through the analytics workflow.
- **Apache Spark** : Provides a powerful, distributed computing engine for large-scale data processing, supporting complex transformations and analytics with high performance and scalability

## Getting Started with Lab

Welcome to your Real Time Analytics with Synapse Workshop! We've prepared a seamless environment for you to explore and learn about Azure services. Let's begin by making the most of this experience.

## Accessing Your Lab Environment
 
Once you're ready to dive in, your virtual machine and lab guide will be right at your fingertips within your web browser.

   ![](../media/gg_1upd.png)

## Exploring Your Lab Resources
 
To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab.

   ![](../media/gg_2upd.png)

## Utilizing the Split Window Feature
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Top right corner.
 
   ![](../media/gg_3upd.png)

## Managing Your Virtual Machine
 
Feel free to **Start, Stop, or Restart** your virtual machine as needed from the **Resources** tab. Your experience is in your hands!

   ![](../media/gg_4upd.png)

## Lab Guide Zoom In/Zoom Out
 
To adjust the zoom level for the environment page, click the **A↕: 100%** icon located next to the timer in the lab environment.

   ![](../media/new-get-start-25-6.png)

## Let's Get Started with Azure Portal

1. In the LabVM, click on the **Azure Portal** shortcut of the Microsoft Edge browser, which is created on the desktop.

      ![](../media/gg_5upd2.png)

1. On the **Sign in to Microsoft Azure** tab, you will see the login screen. Enter the following email/username and click **Next**.

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>

        ![](../media/sc900-image-1upd.png)

1. Now enter the following temporary access pass and click on **Sign in**.

   - **Temporary Access Pass:** <inject key="AzureAdUserPassword"></inject>

       ![](../media/azurepassword.png)

1. If you see the pop-up **Stay Signed in?**, select **No**.

1. If a **Welcome to Microsoft Azure** popup window appears, click **Cancel** to skip the tour.

1. In the search results pane, select **Resource groups**.

   ![15](../media/GS6.png?raw=true)

1. On the **Resource groups** page, you can view the pre-deployed resource group **analyticsSolution**.

   ![16](../media/GS7.png?raw=true)
 
1. Click Next from the bottom right corner to embark on your Lab journey!

Now you're all set to explore the powerful world of technology. Feel free to reach out if you have any questions along the way.

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

### Happy Learning!!
