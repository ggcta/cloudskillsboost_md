---
id: 480
name: 'Analyzing and Visualizing Data the Google Way'
type: Course
url: https://www.cloudskillsboost.google/course_templates/480
date_published: 2022-12-20
topics:
  - Data
---

# [Analyzing and Visualizing Data the Google Way](https://www.cloudskillsboost.google/course_templates/480)

**Description:**

This learning experience guides you through the process of utilizing various data sources and multiple Google Cloud products (including BigQuery and Google Sheets using Connected Sheets) to analyze, visualize, and interpret data to answer specific questions and share insights with key decision makers.

**Objectives:**

* Describe how data analysts use BigQuery and Google Sheets together (via Connected Sheets) to answer data-related questions.
* Use BigQuery and Google Sheets together (via Connected Sheets) to collaborate on data clean-up, analysis, and visualization.

## Using the BigQuery data connector

This module details how Google Sheets engages with data in BigQuery and how data analysts use these products together to answer data-related questions and share insights with stakeholders. At the end of the module, you also have the opportunity to complete an optional challenge lab to test your new skills!  Accessibility considerations: screen reader-friendly player and slide-by-slide audio transcripts included for each lesson

### Link - [Asking the data question](https://www.cloudskillsboost.google/course_templates/480/documents/355347)

* [Asking the data question](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-GOOGAV-B/M1/1_asking_the_data_question/story.html)

### Quiz - [Lesson 1 Quiz](https://www.cloudskillsboost.google/course_templates/480/quizzes/355348)

#### Quiz 1.

> [!important]
> **What are the potential reasons that an organization may have data in BigQuery that has not yet been modeled in Looker? (Please select two choices.)**
>
> * [ ] The datasets are not widely used by multiple teams across the organization.
> * [ ] All BigQuery data must be modeled in Looker.
> * [ ] There is no immediate need to curate custom business intelligence or analytics experiences using that data.
> * [ ] The data are used by too many teams across the organization.

#### Quiz 2.

> [!important]
> **Siobhan has asked Kaveh to identify the top 100 counties with the highest number of people who could benefit from the new solar energy grant.  Based on the grant criteria outlined previously, who can benefit from the grant?**
>
> * [ ] All homeowners in the U.S.
> * [ ] Renters and homeowners with annual incomes below 60,000 USD
> * [ ] All renters and homeowners in the U.S.
> * [ ] Homeowners in the U.S. with annual incomes below 60,000 USD and with homes built before 1960

### Link - [Pulling data into Google Sheets](https://www.cloudskillsboost.google/course_templates/480/documents/355349)

* [Pulling data into Google Sheets](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-GOOGAV-B/M1/2_pulling_data_into_sheets/story.html)

### Quiz - [Lesson 2 Quiz](https://www.cloudskillsboost.google/course_templates/480/quizzes/355350)

#### Quiz 1.

> [!important]
> **When adding a BigQuery data connection to Google Sheets, which type of asset do you choose after selecting a Google Cloud project?**
>
> * [ ] Google Cloud subproject
> * [ ] BigQuery schema
> * [ ] BigQuery dataset
> * [ ] BigQuery table or view

#### Quiz 2.

> [!important]
> **What was the primary reason that you reduced the number of rows of data in the BigQuery table to 10,000?**
>
> * [ ] Focus on the most relevant data, while also making sure the data stays within the row limit
> * [ ] Improve the performance of pulling data from BigQuery into Google Sheets
> * [ ] BigQuery Connected Sheets only supports up to 10,000 rows of data
> * [ ] Reduce the billing cost of pulling data from BigQuery into Google Sheets

### Lab - [Pulling BigQuery Data into Google Sheets using BigQuery Connected Sheets](https://www.cloudskillsboost.google/course_templates/480/labs/355351)

In this lab, you use the BigQuery data connector to pull data from BigQuery tables (in a Google Cloud project) into Google Sheets.

* [ ] [Pulling BigQuery Data into Google Sheets using BigQuery Connected Sheets](../labs/Pulling-BigQuery-Data-into-Google-Sheets-using-BigQuery-Connected-Sheets.md)

### Link - [Priming the data for analysis](https://www.cloudskillsboost.google/course_templates/480/documents/355352)

* [Priming the data for analysis](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-GOOGAV-B/M1/3_priming_data_for_analysis/story.html)

### Quiz - [Lesson 3 Quiz](https://www.cloudskillsboost.google/course_templates/480/quizzes/355353)

#### Quiz 1.

> [!important]
> **What is the maximum number of rows that a Google Sheets data extraction supports?**
>
> * [ ] 74,000 rows
> * [ ] 25,000 rows
> * [ ] 10,000 rows
> * [ ] 30,000 rows

#### Quiz 2.

> [!important]
> **If the data question changes, or the inital selection of columns provides either an incorrect or incomplete answer to the data question, which next step can you take to address this?**
>
> * [ ] Start the entire process over by recreating the data connections using BigQuery Connected Sheets in a new Google Sheets workbook.
> * [ ] Delete the correct extraction and create a new one.
> * [ ] Change the column sort order in the extraction.
> * [ ] Modify the current extraction by adding, removing, or modifying columns using the Extract editor.

### Lab - [Extracting and Filtering BigQuery Data using Google Sheets](https://www.cloudskillsboost.google/course_templates/480/labs/355354)

In this lab, you extract and filter BigQuery data in Google Sheets.

* [ ] [Extracting and Filtering BigQuery Data using Google Sheets](../labs/Extracting-and-Filtering-BigQuery-Data-using-Google-Sheets.md)

### Link - [Performing the data analysis](https://www.cloudskillsboost.google/course_templates/480/documents/355355)

* [Performing the data analysis](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-GOOGAV-B/M1/4_performing_data_analysis/story.html)

### Quiz - [Lesson 4 Quiz](https://www.cloudskillsboost.google/course_templates/480/quizzes/355356)

#### Quiz 1.

> [!important]
> **What is the recommended configuration order when working with columns in a data extraction?**
>
> * [ ] Add columns, Filter by columns, Sort by columns.
> * [ ] Sort by columns, Add columns, Filter by columns.
> * [ ] Add columns, Sort by columns, Filter by columns.
> * [ ] Filter by columns, Sort by columns, Add columns.

#### Quiz 2.

> [!important]
> **If you wanted to reference a specific cell, C95 from the extraction "Extract 1" in a new sheet in the workbook, which is the correct formula to achieve this?**
>
> * [ ] "=LEFT(C95,5)"
> * [ ] "='Extract1'C95"
> * [ ] "='Extract1'!REF(C95)"
> * [ ] "='Extract1'!LEFT(C95)"

### Lab - [Performing the Data Analysis using Google Sheets](https://www.cloudskillsboost.google/course_templates/480/labs/355357)

In this lab, you perform the data analysis process using various features of Google Sheets.

* [ ] [Performing the Data Analysis using Google Sheets](../labs/Performing-the-Data-Analysis-using-Google-Sheets.md)

### Link - [Sharing insights with others](https://www.cloudskillsboost.google/course_templates/480/documents/355358)

* [Sharing insights with others](https://storage.googleapis.com/cloud-training/cls-html5-courses/T-GOOGAV-B/M1/5_sharing_insights_with_others/story.html)

### Quiz - [Lesson 5 Quiz](https://www.cloudskillsboost.google/course_templates/480/quizzes/355359)

#### Quiz 1.

> [!important]
> **Which are steps involved in sharing a Google Sheets workbook with someone? (Please select two choices.)**
>
> * [ ] Download a copy of the workbook and email it as an attachment.
> * [ ] Select the level of workbook access to grant to a specific person.
> * [ ] Define an end-of-share date for the workbook to revoke access after a specific period of time.
> * [ ] Type or search for the name or email address of the person in the XXX menu.

#### Quiz 2.

> [!important]
> **Which section header in the Chart editor contains configuration options for assigning a new global font for the entire chart?**
>
> * [ ] Chart style
> * [ ] Gridlines and ticks
> * [ ] Chart & axis titles
> * [ ] Series

### Lab - [Visualizing and Sharing Insights using Google Sheets](https://www.cloudskillsboost.google/course_templates/480/labs/355360)

In this lab, you create a basic visualization and then share the entire Sheet with others.

* [ ] [Visualizing and Sharing Insights using Google Sheets](../labs/Visualizing-and-Sharing-Insights-using-Google-Sheets.md)

### Lab - [Analyzing and Visualizing Data the Google Way: Challenge Lab](https://www.cloudskillsboost.google/course_templates/480/labs/355361)

In this challenge lab, you use BigQuery Connected Sheets to pull data from BigQuery into Google Sheets in order to perform data analysis to answer a data-related question.

* [ ] [Analyzing and Visualizing Data the Google Way: Challenge Lab](../labs/Analyzing-and-Visualizing-Data-the-Google-Way-Challenge-Lab.md)

## Course Resources

This module provides the student PDF links to all lessons.

### Document - [Course Resources](https://www.cloudskillsboost.google/course_templates/480/documents/355362)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
