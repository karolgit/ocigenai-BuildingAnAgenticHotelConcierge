# OCI Generative AI Workshop: Enhance Guest Experience in Hospitality

## Introduction

This lab focuses on how hotels can enhance guest experiences using **OCI Generative AI**.  
You will step into the shoes of Maria, the General Manager of the Grand Plaza Hotel in Ho Chi Minh City, who receives multilingual reviews daily. With AI, you will learn to summarize reviews, analyze guest sentiment, and translate feedback into English helping managers act quickly and effectively.

Estimated Time: 15–20 minutes

### Objectives

In this lab, you will:

- Use OCI Generative AI to **summarize reviews** in their original language.
- **Analyze sentiment** understand if guest's review is either Positive, Negative, or Neutral.
- **Translate reviews** from non-native languages to staff's native language (eg: English)
- **Respond** to reviews with full context and sentiment understanding
- Understand how AI improves **response times**, **guest satisfaction**, and **revenue**.

### Dataset

We will use the trimmed multi-language TripAdvisor Hotel Reviews dataset from [Zenodo / NIAID ](https://data.niaid.nih.gov/resources?id=zenodo_7967493), and a trimmed CSV version of the dataset is also provided in the repository.

Estimated Time:  15-20 minutes

---

## Task 1: Get Your Sample Text

1. Right-click the [TripAdvisorReviewsMultiLang.csv](./datasets/TripAdvisorReviewsMultiLang.csv) link, select “Save As” to download it to  your local folder. Open the downloaded CSV file in Microsoft Excel from your local folder.

2. Copy one **non-English review** (e.g., Vietnamese, ).
![Alt text](./images/copyinputdata.png "Input Data")

---

## Task 2: Navigate to the OCI Generative AI Playground
 
1. In the **OCI Console**, go to: **Analytics & AI → 'Generative AI' in AI Services **.  

![Alt text](./images/AIServices-GenAI-Link.png "Gen AI Services")

2. Click **Go to Playground** or **Playground-->Chat** in the sidebar to open the interactive interface.

![Alt text](./images/GoToPlayground.png "Playground")

---

## Task 3: Summarize and Analyze the Review

1. In the Playground, select a **Grok model** (e.g. xai.grok-3). Grok is a strong multilingual capabilities.  

![Alt text](./images/SelectGrok-4.png "Select Grok-4")

2. Use the following prompt with your chosen review and click **Submit**.

   ```
   <copy>
   Analyze the hotel review below.
   Provide a one-paragraph summary of the review in its original language.
   In English, identify the sentiment as Positive, Negative, or Neutral.

   Here is the review:
   [PASTE THE NON-ENGLISH REVIEW TEXT HERE]
   </copy>
   ```

   (e.g.)

   ```
   <copy>
   Analyze the hotel review below.
   Provide a one-paragraph summary of the review in its original language.
   In English, identify the sentiment as Positive, Negative, or Neutral.

   Here is the review:
- Nằm ở số 4 Tôn Đức Thắng (trong khu villa cao cấp) và đối diện sông Trà Khúc, cách trung tâm thành phố Quảng Ngãi khoảng 2-3 km. Khách sạn Hana Riverside là một lựa chọn tuyệt vời cho sự riêng tư. - Đây thực chất là 1 dạng villa và kinh doanh các phòng
   </copy>
   ```

   ![Alt text](./images/EnterInputAndSubmit.png "Enter Input And Submit")
   

3. The model outputs a summary in the **original language** plus sentiment analysis.

   ![Alt text](./images/SentimentofReview.png "Sentiment of Review")

---

## Task 4: Translate the Review

1. Use the same chat from Task 4
2. Use the following prompt and click  **Submit** to get a full English translation:

   ```
   <copy>
   Translate the hotel review into English
   </copy>
   ```

   The model outputs the translated summary in  **English language**  
   ![Alt text](./images/TranslatedText.png "Output - TranslatedText")

## Task 4.1: Generate a response
1. Use the same chat from Task 4
2. Use the following prompt and click  **Submit** to get a response using the original user review and sentiment

   ```
   <copy>
   Based on the guest review and the sentiment, generate a response for Maria, on behalf of the hotel
   </copy>
   ```
   
### Conclusion & Value

Maria and her team used to spend hours every day reading reviews in different languages, translating them, trying to understand what guests were really saying, and then writing thoughtful responses—all while struggling to keep up with the volume.  

- **Analyzed** guest reviews in foreign languages and identified sentiment  
- **Translated** reviews into the team’s native language (e.g., English)  
- **Responded** with clear, empathetic messages that reflected full understanding of the guest’s feedback  

### Business Impact  

- **Time savings**: Responses go out in minutes instead of days  
- **Accuracy**: AI captures nuance and cultural context even in non-native languages  
- **Automation**: Fewer mistakes, less manual work, and more time for staff to focus on guests and operations  
- **Scalability**: Handles growing review volume without adding headcount, while improving response times  

In this Lab, we delivered Maria and her team a simple solution that directly impacts the company’s bottom line—better service for guests, improved working conditions for employees, and higher returns on investment.  

### What's Next
In **Lab 2**, you will build an **AI Concierge** capable of analyzing thousands of reviews at once, uncovering patterns, and recommending actions.  
This step moves you beyond single-review analysis into **strategic intelligence** for hospitality management powered by OCI Generative AI Agents.


---

## Acknowledgements  

**Authors:**  
- Felipe Garcia, Master Principal Cloud Architect 
- Karol Stuart, Master Principal Cloud Architect  

**Last Updated by/Date** – Karol Stuart, August 2025  
