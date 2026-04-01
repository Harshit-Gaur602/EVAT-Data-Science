# Voice Assistant Use Case – Data Science Perspective

## 1. Context

The EVAT system currently provides working capabilities for:

- Congestion prediction  
- Wait time estimation  
- Cost comparison  

These features are accessible through a dashboard and are supported by existing data processing and prediction models.

---

## 2. Current Capability

At present, the system:

- Loads and processes structured data  
- Generates predictions for charger usage and wait times  
- Displays results through an interactive dashboard  
- Supports basic scenario analysis  

This establishes a strong analytical foundation.

---

## 3. Gap for Voice Assistant Use Case

While the system performs well analytically, it does not yet support natural language interaction.

The following capabilities are not present:

- Understanding user questions  
- Extracting useful information from queries  
- Connecting queries to prediction models  
- Generating simple, conversational responses  

As a result, the system operates as a dashboard rather than an interactive assistant.

---

## 4. Steps to Enable Voice Assistant Functionality

To support a voice assistant use case, the following components can be introduced:

---

### 4.1 Intent Detection

User queries can be categorized based on their purpose, such as:

- Congestion-related queries  
- Cost-related queries  
- General or unsupported queries  

A simple rule-based approach can be used initially for fast and reliable implementation.

---

### 4.2 Entity Extraction

Key details can be extracted from user queries, including:

- Location (e.g., charger station)  
- Distance (for cost estimation)  

This allows dynamic input generation instead of relying on predefined values.

---

### 4.3 Integration with Existing Models

Extracted information can be passed to existing EVAT models:

- Congestion model → provides wait time and charger status  
- Cost model → provides EV vs petrol comparison  

This enables reuse of current system capabilities without modifying core models.

---

### 4.4 Response Generation

Model outputs can be converted into simple, user-friendly responses.

Examples:

- “The charger is moderately busy with a short wait time.”  
- “The estimated cost for your trip is lower for EV compared to petrol.”  

---

### 4.5 Logging and Evaluation

Basic logging can be introduced to capture:

- User queries  
- Detected intent  
- Extracted information  
- Generated responses  

This supports evaluation and continuous improvement.

---

## 5. Integration Consideration

The interaction layer (such as a chatbot or voice interface) is expected to integrate with the data science components for query processing and response generation.

This ensures clear separation between user interface and backend logic.

---

## 6. Approach Considerations

The proposed approach is designed to be:

- Simple to implement  
- Compatible with the current EVAT system  
- Independent of complex machine learning models  
- Suitable for incremental development  

This allows gradual transition from a dashboard-based system to an interactive assistant.

---

## 7. Expected Outcome

With the addition of these components:

- Users can interact with the system using natural language  
- Existing models can be accessed more intuitively  
- The system evolves into an interactive tool  

---

## 8. Summary

The EVAT system already provides strong analytical capabilities.

By introducing a lightweight interaction layer that supports query understanding and response generation, the system can be extended towards a voice assistant use case without major changes to the existing architecture.