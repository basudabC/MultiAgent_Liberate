# Multi-Agent Competitor Analysis System

This project demonstrates a multi-agent system designed for competitor analysis and market research. The system uses advanced LLM (GROQ), modular frameworks (Phidata), and efficient data handling strategies to produce comprehensive competitor reports.

---

## **Overview**
The system is built to:
1. Retrieve product, company, and competitor details.
2. Aggregate data from diverse sources like Google, Crunchbase, and Reddit.
3. Analyze sentiment, perform SWOT analyses, and synthesize insights.
4. Generate actionable reports for business decision-making.

---
## **Run the project**
Install the necessary dependencies:
pip install -r requirements.txt
 API keys:

A dot.env file is included in the project.
Make sure to remove the **dot** from the file name so that it is recognized as **.env**.
All of the API keys included in the dot.env file.
Run the project: You can also run the project in Google Colab: [Google Colab Link](https://colab.research.google.com/drive/19sEmpqi2u-EQuyobtbkcTcrWl5FiCjOi?usp=sharing)

If you're using Colab:

Open the provided Google Colab link.
Follow the instructions inside the Colab notebook to set up and run the project.
## **System Architecture**

### **Agents Overview**
- **Web Search Agent**:
  - Searches for product/company details and similar services/products.
  - Passes organization names to the next agent.

- **Crunch Agent**:
  - Reads the provided organization names.
  - Prepares detailed reports on each organization.

- **Reddit Agent**:
  - Analyzes user sentiment and trustworthiness for the organizations.
  - Passes findings to the Summary Writer.

- **Summary Writer**:
  - Synthesizes data from the Crunch and Reddit agents.
  - Identifies trends, strategies, and competitor insights.

- **Team Agent**:
  - Consolidates all outputs into a final report.

### **Data Flow**
1. **Web Search Agent** → Searches for organization and product details.
2. **Crunch Agent** → Reads organization names and prepares detailed data.
3. **Reddit Agent** → Analyzes sentiment and passes it forward.
4. **Summary Writer** → Consolidates all agent outputs.
5. **Team Agent** → Produces the final comprehensive report.

---

## **Technologies Used**

### **1. Chosen LLM: GROQ**
- **Why GROQ?**
  - Contextual understanding for complex queries.
  - Summarization of large text inputs into actionable insights.
  - Scalability for handling large datasets.
  - High accuracy for NLP-driven tasks.

---

### **2. Framework: Phidata**
- **Why Phidata?**
  - Modular design for creating reusable agents.
  - Seamless data flow orchestration between agents.
  - Scalable and distributed architecture for handling large data volumes.
  - Robust error handling to address conflicts and missing values.

---

### **3. Data Handling Strategies**
- **Data Integration**:
  - Ingests data from multiple sources (Google, Crunchbase, Reddit).
  - Normalizes data for consistency and accuracy.

- **Conflict Resolution**:
  - Resolves conflicting information by assigning confidence scores.

- **Sentiment Analysis**:
  - Leverages Reddit data to understand user perspectives on products/services.

- **Summarization**:
  - Synthesizes all data into trends, strategies, and market insights.

- **Final Report**:
  - Consolidates outputs into actionable insights for decision-making.

---

## **How It Works**
### **Instructions for Agents**
1. **Web Search Agent**:
   - Searches for product/company details and similar services/products.
   - Sends organization names to the Crunch Agent.

2. **Crunch Agent**:
   - Reads organization data and prepares detailed reports.

3. **Reddit Agent**:
   - Reads organization names and analyzes user sentiment.
   - Passes sentiment data to the Summary Writer.

4. **Summary Writer**:
   - Consolidates data from Crunch and Reddit agents.
   - Identifies trends, strategies, and opportunities.

5. **Team Agent**:
   - Combines all outputs into a detailed business report.

---

## **System Output**
The system produces:
- A detailed competitor analysis report.
- SWOT analyses, feature comparisons, and user sentiment insights.
- Strategic recommendations for market positioning.

---

## **Key Advantages**
1. **Modular and Scalable**:
   - Easy to extend and adapt for future requirements.

2. **Accurate and Actionable**:
   - Provides precise and meaningful insights for strategic decisions.

3. **Automated Reporting**:
   - Reduces manual effort while ensuring high-quality output.

---

## **Conclusion**
This multi-agent system is designed to deliver efficient and accurate competitor analysis, leveraging the strengths of GROQ, Phidata, and advanced data strategies. It provides businesses with actionable insights to make informed decisions.

---

## **Contact**
For any inquiries or contributions, feel free to reach out!

