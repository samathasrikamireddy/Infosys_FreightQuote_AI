# 🚢 FreightQuote AI Platform — Milestone 2 

Milestone 2 transitions the platform from a foundational data processing baseline (Milestone 1) into a secure, fully interactive, multi-agent intelligence ecosystem. While Milestone 1 focused on standalone calculations and basic script logic, Milestone 2 builds a unified Streamlit dashboard orchestration layer driven by autonomous agents, secured by localized database authentication, and augmented by a Generative AI executive advisory copilot. 

## 🚀 Key Features Built
	
### Security Gateway Lockout: 
Secure User Authentication (Login, Register, Password Recovery) utilizing Gmail OTP verification, role-based routing (User vs Admin), and progressive account lockout mechanics (3/4/5 failed attempts leading to temporary 5-min, 15-min, or permanent admin-controlled lockouts) enforced via an SQLite backend. 

### Domain Intelligence Engine: 
Three autonomous tabular reasoning modules providing real-time operational forecasting: 
	
#### Agent 1 (Dynamic Freight Pricing): Predicts dynamic shipping rates based on container types, fuel indices, and seasonal demand variations (evaluated across 5+ algorithms with R^2≥0.90). 
	
#### Agent 2 (Route Delay Classifier): Classifies potential shipping delays based on historical port congestion, weather conditions, and transit vectors (optimized for ROC-AUC across 5+ models). 
	
#### Agent 3 (Carrier Compliance Sentinel): Evaluates maritime carrier risk profiles, insurance updates, and regulatory compliance flags (optimized for ROC-AUC across 5+ models). 

### Generative Executive Advisory: 
A centralized LLM Copilot (powered by quantized local models like Qwen2.5-3B-Instruct or Gemini APIs) that ingests the structured mathematical outputs of the three autonomous agents and synthesizes them into actionable shipping strategy briefs and structured JSON logistics audits. 

### System Administration Controls: 
An isolated administrative control panel allowing user role management (Add/Delete/Unlock workflows), system telemetry logs, and manual security overrides. 


## 🛠️ Tech Stack Used
	
Core UI & Orchestration: Streamlit (v1.35.0+) 
	
Database & Storage: SQLite3 (State retention & user credentials) 
	
AI Engine & Tooling: Hugging Face Transformers, BitsAndBytes (4-bit quantization), PyTorch, Google GenAI SDK 
	
Security & Encryption: PyJWT, Bcrypt (Password hashing), SMTPLIB (Gmail OTP transport) 
	
Data Processing & ML: Pandas, NumPy, Scikit-Learn, Joblib 
	
Tunneling: Pyngrok 


