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

6. `Diff_Between_Loghub1_Loghub2_Hadoop_OpenStack.csv`: This CSV file captures the differences between LogHub 1.0 and LogHub 2.0 for Hadoop and OpenStack projects. It includes the following columns:
   - `Project`: Name of the project associated with the log template. The value here is either OpenStack or Hadoop.
   - `EventId`: Represents the unique identifier for a log template. The format depends on the version of LogHub where the template was found:
      - For **LogHub 1.0**, the EventId has no prefix (e.g., `E30`).
      - For **LogHub 2.0**, the EventId includes a prefix (e.g., `Loghub2.0-E48`).
   - `EventTemplate`: The actual log template text associated with the EventID.
   - `Differ`: Indicates where the log template differences were found. Possible values are:
      - `in our manuscript (manually validated with log templates summarized by Drain3)`: The log template was identified and used in our manuscript.
      - `in loghub2.0`: The log template was provided by LogHub 2.0.
   - `Note`: Explains the reason for the difference. Examples include:
      - `missing by us`: Indicates the log template was missed during our manual validation of Drain3 results.
      - `different full log dataset`: Indicates the difference arose due to changes in the full log datasets used in Loghub1.0 and Loghub2.0.
   - `ManualEmotion`: Manually annotated emotion for the log template.

7. `Loghub2.0_Thunderbird_294Samples.csv`: This CSV file includes a representative sample of 294 log templates for the Thunderbird project in Loghub2.0, selected to ensure a 95% confidence level. It includes the following columns:
- `EventId_In_Loghub2.0`: The unique identifier for each log template.
- `EventTemplate`: The actual text of the log template associated with the Event ID.
- `ManualEmotion`: Manually annotated emotion for the log template.
