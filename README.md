\#College Admission RAG Bot 🎓🤖



A Retrieval-Augmented Generation (RAG) powered chatbot built with IBM Watsonx.ai and IBM Granite foundation model. The bot helps streamline college admission inquiries by retrieving accurate and up-to-date information from institutional data sources like admission policies, eligibility criteria, fee structure, courses, and deadlines.



Built using:



\* IBM Watsonx.ai Prompt Lab

\* IBM Granite-3-3-8b-instruct LLM

\* Grounded with document-based knowledge

\* Deployed as an AI service with public API access



📌 Features



\* Ask natural language questions about:



&nbsp; \* Admission eligibility

&nbsp; \* Fee structure

&nbsp; \* Course offerings

&nbsp; \* Important dates and deadlines

&nbsp; \* Application procedures



\* Powered by IBM Granite foundation model for accurate generation



\* Grounded with trusted .txt documents for factual responses



\* Deployable and accessible via RESTful API (JavaScript, Python, etc.)



📂 Project Structure



├── assets/                   # Upload files used in Prompt Lab (college\\\_admission\\\_info.txt)

├── deployment/               # Contains API endpoints and integration scripts

│   └── JavaScript\\\_sample.js  # Example JS code to access the bot via API

├── docs/                     # Presentation and documentation

│   └── Project\\\_Presentation.pptx

├── README.md



🚀 How It Works



1\. Upload Admission Data:



&nbsp;  \* A .txt file with verified college information was uploaded to Prompt Lab.

&nbsp;  \* Example: college\\\_admission\\\_info.txt



2\. Prompt Configuration:



&nbsp;  \* The prompt defines the bot's role as a helpful admission agent.

&nbsp;  \* Example Prompt:

&nbsp;    "You are an admission assistant. Answer questions based on the uploaded document using clear and factual language."



3\. Model \& Runtime:



&nbsp;  \* Model: granite-3-3-8b-instruct

&nbsp;  \* Runtime: Watsonx.ai with grounding support



4\. Deployment:



&nbsp;  \* Prompt deployed as an AI service in IBM Cloud.

&nbsp;  \* Space: CollegeAdmission\\\_RAG\\\_Bot

&nbsp;  \* Deployed using: Deployment Notebook

&nbsp;  \* API Endpoint generated for external access.



🛠️ How to Use



Step 1: Get API Key



\* Go to IBM Cloud IAM → Generate an API Key.



Step 2: Authenticate \& Call API



JavaScript Sample:

const API\\\_KEY = "\\<your\\\_api\\\_key>";

const scoring\\\_url = "\\<your\\\_public\\\_endpoint>";

// Authenticate and send a POST request with question payload



Payload format:

{

"messages": \\\[

{ "role": "user", "content": "What is the eligibility for B.Tech CS?" }

]

}



Step 3: Receive Response



\* JSON output with grounded and context-aware response.



📊 Evaluation



\* Accuracy: Grounded answers based on institutional data

\* Transparency: Source-aware responses reduce misinformation

\* Accessibility: Deployed as a scalable API or embedded in web UI



🧠 Future Enhancements



\* Add support for PDF/HTML parsing in Watsonx.ai

\* Integrate user session memory for contextual chats

\* Build a React-based UI for interactive college counseling

\* Fine-tune Granite model with domain-specific examples (if supported)



📄 License



This project is developed under the guidelines of SmartBridge x IBM Edunet Hackathon 2025. Educational and prototype use only.



🙌

