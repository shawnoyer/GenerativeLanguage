# GenerativeLanguage
Contains a project done on Generative Language for CS 614 at Drexel University

Title: Automated Hotel Review Summarization Using Generative AI: Assessing BART versus T5-small Models

Created By: Shawn Oyer on 9/3/2024

Abstract:  The adoption of Generative AI has transformed the travel industry, particularly in enhancing customer experience and operational efficiency. This project investigates the application of AI-driven text summarization models, specifically BART and T5-small, to generate concise summaries of hotel reviews from a large dataset scraped from booking.com. The models were evaluated using ROUGE metrics, which assess the quality of the generated summaries by comparing them to human-created summaries. The results demonstrate that the BART model significantly outperforms the T5-small model across all ROUGE metrics, indicating its superior ability to capture key contextual information while maintaining the structural integrity of the original reviews. This research highlights the potential of advanced text summarization models like BART in summarizing user-generated content, thereby creating more efficient information retrieval and enabling more informed decision-making processes in the travel sector.

Data: The data can be downloaded here:
https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe

The data consists of a .CSV file with 515,000 customer reviews and ratings of 1493 luxury hotels across Europe scraped from Booking.com in 2017. Here are the 17 fields and descriptions:

Hotel_Address: Address of hotel.
Review_Date: Date when reviewer posted the corresponding review
Average_Score: Average Score of the hotel, calculated based on the latest comment in the last year
Hotel_Name: Name of Hotel
Reviewer_Nationality: Nationality of Reviewer
Negative_Review: Negative Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Negative'
Review_Total_Negative_Word_Counts: Total number of words in the negative review
Positive_Review: Positive Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Positive'
Review_Total_Positive_Word_Counts: Total number of words in the positive review
Reviewer_Score: Score the reviewer has given to the hotel, based on his/her experience
Total_Number_of_Reviews_Reviewer_Has_Given: Number of Reviews the reviewers has given in the past
Total_Number_of_Reviews: Total number of valid reviews the hotel has
Tags: Tags reviewer gave the hotel.
days_since_review: Duration between the review date and scrape date
Additional_Number_of_Scoring: There are also some guests who just made a scoring on the service rather than a review. This number indicates how many valid scores without review in there
lat: Latitude of the hotel
lng: Longitude of the hotel

Contents: The contents of the .ipynb file are separated into the following sections: 

  Proccessing
  Testing Examples
  EDA
  Data Cleaning
  BART Pipeline
  Hyperparameter Tuning with T5-Small Model
 
Stakeholders: Used by hotel management & owners, travel platforms, travelers/tourists, marketing & sales teams, Data Science Teams

Uses and Intensions: Specifically, this project aims at generating text summarizations for thousands of hotel reviews that incorporate user perspectives on key attributes of quality such as location, atmosphere, hospitality and services using two pre-trained summarization models, BART and T5-small.

Using the Script: The extension of the script is .ipynb so it can be accessed and run within jupyter notebook and exported as a .py to export into any Python IDE

Contributors and Contact List: Shawn Oyer - Drexel University Gradate Student, sbo33@drexel.edu

License Information: CC0 1.0 license

Sources:

Garcia-Madurga, Miguel A., and Ana J. Grillo-Mendez. “Artificial Intelligence in the Tourism Industry: An Overview of Reviews.” MDPI, vol. 13, no. 8, 2023, p. 13. MDPI, https://www.mdpi.com/2076-3387/13/8/172. Accessed 30 August 2024.
Gopalakrishnan, Karthika. “TEXT SUMMARIZATION USING GENERATIVE AI: A CASE STUDY IN BANKING INDUSTRY.” iaeme, 2024, https://iaeme.com/MasterAdmin/Journal_uploads/JAIML/VOLUME_3_ISSUE_1/JAIML_03_01_001.pdf. Accessed 30 August 2024.
Hugging Face. “facebook/bart-large-cnn · Hugging Face.” Hugging Face, 18 January 2024, https://huggingface.co/facebook/bart-large-cnn. Accessed 3 September 2024.
Hugging Face. “Falconsai/text_summarization · Hugging Face.” Hugging Face, 2024, https://huggingface.co/Falconsai/text_summarization. Accessed 3 September 2024.
Hugging Face. “Summarization.” Hugging Face, 2024, https://huggingface.co/docs/transformers/en/tasks/summarization. Accessed 30 August 2024.
Lin, Chin Y. “ROUGE: A Package for Automatic Evaluation of Summaries.” ACL Anthology, 2004, https://aclanthology.org/W04-1013.pdf. Accessed 3 September 2024.
Liu, Jiashen. “515K Hotel Reviews Data in Europe.” Kaggle, Kaggle, 2017, https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe/code. Accessed 30 August 2024.
Oluwafemidiakhoa. “Unlocking the Power of Text Summarization: A Comprehensive Guide to Building a Production-Ready Solution with Hugging Face Transformers.” Medium, 8 April 2024, https://medium.com/kinomoto-mag/unlocking-the-power-of-text-summarization-a-comprehensive-guide-to-building-a-production-ready-757585a8fb46. Accessed 30 August 2024.
Payne, Matt. “State of the Art GPT-3 Summarizer For Any Size Document or Format.” Width.ai, 21 August 2023, https://www.width.ai/post/gpt3-summarizer. Accessed 30 August 2024.
Tiernan, Kirstie. “Airbnb has used artificial intelligence & machine learning to disrupt the marketplace to become the fastest-growing hotelier provider in recent years.” BDO USA, 28 August 2023, https://www.bdo.com/insights/digital/airbnb-artificial-intelligence-transform-business. Accessed 30 August 2024.
TripAdvisor. “Tripadvisor Launches AI-Powered Hotel Review Summaries.” Hospitality Net, 25 October 2023, https://www.hospitalitynet.org/news/4118778.html. Accessed 30 August 2024.
Veluru, Chandra S. “Transforming Travel Planning: The Impact of Generative AI on Itinerary Optimization, Cost Efficiency and User Experience.” Journal of Artificial Intelligence & Cloud Computing, vol. 2(4), no. 2754-6659, 2023, pp. 1-8. Research Gate, https://www.researchgate.net/publication/382212715_Transforming_Travel_Planning_The_Impact_of_Generative_AI_on_Itinerary_Optimization_Cost_Efficiency_and_User_Experience. Accessed 30 August 2024.
