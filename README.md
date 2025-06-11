# Architecture Overview

The AI agents leverage Large Language Models (LLMs) for their language understanding and generation capabilities. The system incorporates various frameworks and tools to empower users to build domain knowledge through meta-analyses and identify relevant datasets during the **business understanding** phase. Subsequently, in the **data understanding** phase, users can intuitively perform exploratory analyses on datasets using natural language. The AI agents facilitate the steps of **data extraction** and **processing** of datasets, including the **training** and **evaluation** of machine learning models to allow predictive analysis at scale. A human-in-the-loop approach is employed, requiring code review before execution.

---

![Image](https://github.com/user-attachments/assets/580fa77e-53ae-421f-bf08-1d366b63f30b)

* **N8N** for workflow automation in domain exploration and dataset discovery.
* **AG2 (Autogen)**: Agentic framework to automate the data mining process.
* **Streamlit**: User interface that allows for interaction with the agents.
* **Supabase**: Cloud data storage, agent memory and encrypted user authentication.

### Agent Functionality Across CRISP-DM Phases

Autocrisp is built following the principles of a foundational framework for data mining. The Cross-industry standard process for data mining, known as CRISP-DM, is an open standard process model that describes common approaches used by data mining experts. It is the most widely-used analytics model.

---

![Image](https://github.com/user-attachments/assets/55535a1c-1505-4b97-8780-d1ce1656b4b7)
![Image](https://github.com/user-attachments/assets/872de1c7-e3fb-49e0-a6cb-865864f713fa)

### Integration of Technologies

Autocrisp is utilizing N8N for its business understanding capabilities by connecting the user in foremost with an orchestration agent that can answer direct questions or brainstorm ideas. The orchestration agent may delegate research tasks towards a set of agents capable of automating comprehensive literature research, identifying relevant datasets through targeted web searches and querying datasets using natural language to SQL.

---

![Image](https://github.com/user-attachments/assets/1ab10c9f-f6c5-4dc3-85b4-0a3729eccf85)
![image](https://github.com/user-attachments/assets/5f908cfd-bd4b-48ff-92ac-2036ddc39f04)

The remaining phases data understanding, data preparation, modeling, and evaluation are supported by agents built on the Autogen (AG2) framework. These agents handle tasks such as:

* Exploratory data analysis
* Data cleaning
* Model training
* Model evaluation

All components are integrated into a Streamlit-based application, providing users with an interactive way to engage with the agents.
