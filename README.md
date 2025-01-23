# Quiz Performance Analyzer & Recommendations System

This project analyzes the performance of quiz participants, identifies weak areas, tracks improvement trends, and generates personalized recommendations for improvement based on historical quiz data.

## Project Overview
The Quiz Performance Analyzer fetches quiz data from online APIs, processes the data, calculates performance metrics, and provides personalized recommendations. The system can identify topics where the user is underperforming (weak areas), track their progress over time, and suggest improvements in terms of focus topics and difficulty adjustments.

## Features
Fetch quiz data from a set of public APIs.
Process historical quiz submissions and calculate accuracy for each topic.
Generate insights on weak areas, strong areas, and performance gaps.
Provide actionable recommendations to improve performance based on historical results.
Visualize performance trends via bar charts.

## Tech Stack
Python 3.x
Pandas for data manipulation.
Matplotlib and Seaborn for data visualization.
Requests for making HTTP requests to external APIs.

## API Endpoints
The following public APIs are used to fetch quiz data:
Quiz Data: QUIZ_ENDPOINT_URL
Contains details of available quiz questions.
Quiz Submission Data: QUIZ_SUBMISSION_URL
Contains data on quiz submissions (user answers, scores).
Historical Quiz Data: HISTORICAL_QUIZ_URL
Contains historical data on quiz performances.

## How It Works
1. Fetch Data
The system fetches quiz data, submission data, and historical quiz data from the provided API endpoints.
2. Data Processing
The quiz data is parsed into a DataFrame for easy analysis.
The submission and historical data are processed and merged into a unified format for performance analysis.
3. Performance Analysis
Accuracy is calculated for each quiz and each topic based on the number of correct answers and total questions.
Insights are generated, identifying weak and strong areas, as well as any missing data points (performance gaps).
4. Recommendations Generation
The system provides personalized recommendations:
Focus Topics: Topics where the accuracy is below 50% are identified as weak areas.
Suggested Difficulty: Based on overall performance, the system recommends whether to increase or maintain quiz difficulty.
Improvement Trends: It tracks topics that have shown improvement and those that need more focus.
5. Visualization
A bar chart visualizing the accuracy of each quiz topic is generated using Matplotlib and Seaborn.

## Example Output
The system outputs personalized recommendations based on quiz performance, including:
Weak Areas: Topics where the user has low accuracy.
Strong Areas: Topics where the user has shown strong performance.
Performance Gaps: Topics with missing performance data.
Improvement Trends: Topics that have improved or declined over time.
Focus More: Suggests whether the user should focus more on weak topics.
Suggested Difficulty: Recommends whether to adjust quiz difficulty.

## Visualization
The performance across topics is visualized using a bar chart, showing the accuracy for each quiz topic.
