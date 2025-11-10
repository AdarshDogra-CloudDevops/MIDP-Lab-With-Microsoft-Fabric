# Exercise 2: Explore the offline data and analytics pipeline using open Delta format

### Estimated Duration : 60 minutes

Analyzing disparate data sources in an integrated way has been a challenge for Wide World Importers. In the past, different teams at the company were assigned to analyze customer churn, social media trends, marketing campaigns, and sales forecasts. So, it was left to business analysts and executives to synthesize these datasets into a data-driven, decision-making solution. By delivering a Lakehouse, it becomes simpler for teams to collaborate in a unified workspace to process, analyze, and model data.

In this exercise, you will stitch two sets of data together to generate actionable insights. You will set up an Azure Databricks Delta Live Table (DLT) pipeline to build a simple Lakehouse. The pipeline will enrich the data by scoring it with machine learning models to help better understand customers and how to reduce churn.

The data source for the pipeline is the Bronze layer in ADLS Gen2, which was loaded by the Synapse pipeline in Exercise 1. This Bronze layer contains campaign data, customer churn data, store transactions data, sales data, and Twitter messages.

## Objectives

- Task 2.1: Set up Azure Databricks environment
- Task 2.2: Review sentiment analysis model training

## Task 2.1: Set up Azure Databricks environment <a name="adb-env"></a>

1. In the Azure portal web session (tab), in the search box (located across the top of the page), enter **Azure Databricks**.

2. In the search results pane, select **Azure Databricks**.

   ![Select Azure Databricks](../media/image2102.png) 

3. On the **Azure Databricks** page, select the resource named **databricks<inject key="DeploymentID" enableCopy="false"/>**.

   >**Note:** Each user has their own unique instance of this resource. Each Azure Databricks workspace is provisioned with a full-featured development environment.

4. In the Azure Databricks resource page, select **Launch Workspace**.

   ![Launch Workspace](../media/image2104.png) 

   *A new web session (tab) will open. Now, set up the Databricks compute ready to serve your workload.*

   >**Note:** If a pop-up appears, select **Close**.

5. Select **Workspace (1)** from the left navigation pane, click on **Workspace (2)** folder and Select the **ADB_Initial_Setup (3)** notebook.

   ![](../media/new-real-time-feb-12.png)

   > **Note: DO NOT** run this script. 
   > This image is for informational purposes only. 
   > Due to time constraints, we will not run this notebook in the lab session.

   *In exercise 1, we extracted data from a spectrum of data sources and landed it into the ADLS Gen2 data lake. To access this data from the ADLS Gen2 data lake, we need to mount it on the Azure Databricks filesystem. Executing this script will mount ADLS Gen2 to Azure Databricks.*

---

## Task 2.2: Review sentiment analysis model training. <a name="sentiment-model"></a>

In this task, you will explore the sentiment analysis model training notebook. This notebook is used to retrieve the model ID that’s used by the DLT pipeline for further data processing.

*Sentiment Analysis is a branch of Natural Language Processing where text is contextually mined to identify and extract subjective information in the source material to understand whether the underlying sentiment is positive, negative, or neutral.*

1. To open a different workspace, select **Workspace (1)** from the left navigation pane, click on **Workspace (2)** folder and Select the **02_Twitter_Sentiment_Score_Pred_Custom_ML_Model (3)** notebook.

   ![](../media/04/midp-img-2.png)

   > **Note: DO NOT** run this script.

   *Running this script will generate an ML model ID. This Model ID is used by the Delta Live Pipeline* 

## Summary

In this exercise, You have set up a solid foundation of fully stitched data comprised of campaign data and Twitter data from disparate sources, including some key data transformations.

### You have successfully completed the lab. Click on **Next >>** to procced with next exercise.
