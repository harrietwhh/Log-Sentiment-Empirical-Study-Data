# Log and Issue Data

## Overview
This repository contains several CSV files that store information about log templates, issue sentences, issue reports, and their corresponding manual annotations of emotion and sentiment.

## Files
1. `Lohgbub_log_emotion_sentiment.csv`: This file contains log template data with the following columns:
   - `NO.`: Sequential number of the log templates.
   - `Project`: Name of the project associated with the log template.
   - `EventTemplate`: Log templates.
   - `Manual_Emotion`: Manually annotated emotion for the log template.
   - `Manual_Sentiment`: Manually annotated sentiment for the log template.

2. `IssueData_issue_sentence_manual_sentiment.csv`: This file contains issue sentence data with the following columns:
   - `Filename`: Name of the file associated with the issue sentence.
   - `Sentence`: Text of the issue sentence.
   - `Manual_Sentiment`: Manually annotated sentiment for the issue sentence.

3. `IssueData_issue_description_manual_emotion_and_sentiment.csv`: This file contains issue report data with the following columns:
   - `Filename`: Name of the file associated with the issue report.
   - `IssueReport`: Text of the issue report.
   - `ManualEmotion`: Manually annotated emotion for the issue report.
   - `Manual_Sentiment`: Manually annotated sentiment for the issue report.

4. `RQ3_potential_critical_logs_and_its_issue_reports.csv`: This file contains data related to potential critical logs and their associated issue reports, with the following columns:
   - `Filename`: Name of the file associated with the logs.
   - `Log_Level`: Verbosity level of the logs.
   - `Tools_Senti_Emo`: Tools' sentiment and emotion annotations for the log-related issue reports.

5. `RQ3_critical_logs_and_its_issue_reports.csv`: This file contains data related to critical logs and their associated issue reports, with the following columns:
   - `Filename`: Name of the file associated with the logs.
   - `Log_Level`: Verbosity level of the logs.
   - `Tools_Senti_Emo`: Tools' sentiment and emotion annotations for the log-related issue reports.
   - `Manual_Senti_Emo`: Manually annotated sentiment and emotion for the log-related issue reports.
   - `Concerns`: Concerns associated with the logs and issue reports.