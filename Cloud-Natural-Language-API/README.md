# Cloud Natural Language API

## Objective  
This lab demonstrated how to use the Cloud Natural Language API to extract entities, analyze sentiment, evaluate syntax, and process multilingual text. The focus was on building API requests with curl, understanding responses, and applying different analysis methods on text samples.

---

## Tools & Services Used  
- Cloud Natural Language API  
- Compute Engine (Linux instance for curl requests)  
- API Key authentication  
- curl for REST API calls  

---

## Steps Performed  
1. **Created an API key** in the Cloud Console and exported it as an environment variable for authentication.  
2. **Made an entity analysis request** using JSON input and `analyzeEntities`, identifying people, places, and objects within a sentence.  
3. **Performed sentiment analysis** with `analyzeSentiment`, retrieving both document-level and sentence-level sentiment scores and magnitudes.  
4. **Analyzed entity sentiment** with `analyzeEntitySentiment`, distinguishing positive and negative sentiment toward specific entities in text.  
5. **Explored syntax analysis** with `analyzeSyntax`, extracting parts of speech, lemmas, and dependency trees from a sample sentence.  
6. **Tested multilingual analysis** by submitting Japanese text, confirming automatic language detection and appropriate entity extraction with Wikipedia metadata.  

---

## Key Learnings  
- The Natural Language API provides multiple modes of analysis: entities, sentiment, entity-level sentiment, and syntax.  
- Sentiment is expressed through two metrics: **score** (-1 to 1) and **magnitude** (intensity of sentiment).  
- Entity sentiment analysis gives more detailed insight than document sentiment, especially for reviews and opinion-rich text.  
- Syntax analysis reveals linguistic structure, including part of speech and dependencies between words.  
- The API supports multiple languages and automatically detects them.  

---

## Real-World Application  
The Cloud Natural Language API is useful in real-world scenarios such as:  
- Analyzing customer reviews to identify sentiment toward products and services.  
- Classifying user feedback into themes using entity recognition.  
- Powering chatbots and virtual assistants with language understanding.  
- Processing multilingual text for global applications without separate pipelines.  

---

## Reflection  
This lab provided a comprehensive overview of the Natural Language API’s capabilities. I gained practical experience in building requests and interpreting JSON responses. I especially found the entity-level sentiment analysis valuable for use cases like customer experience monitoring. The multilingual capability reinforced how the API can scale across diverse datasets.
