# Concept Dependencies: Directed Acyclic Graph (DAG)
## Learning Path Structure for AI Integration in Non-Profits

### Overview
This document maps prerequisite relationships between the 200 concepts, ensuring learners encounter concepts only after mastering their dependencies. The structure forms a Directed Acyclic Graph (DAG) where arrows indicate "must learn before" relationships.

---

## TIER 1: FOUNDATION (No Prerequisites)
These concepts have no dependencies and can be learned first.

**Tier 1 Concepts:**
- 001: Artificial Intelligence (AI)
- 007: Algorithm
- 091: 501(c)(3)
- 092: Mission Statement
- 096: Beneficiary
- 097: Donor
- 189: Cloud Computing
- 190: SaaS

---

## TIER 2: BASIC UNDERSTANDING
These concepts require only Tier 1 knowledge.

### AI Foundations Branch
**002: Machine Learning** ← 001 (AI)
**004: Natural Language Processing** ← 001 (AI)
**005: Computer Vision** ← 001 (AI)
**031: Generative AI** ← 001 (AI)

### Data & Privacy Branch
**071: Data Privacy** ← 001 (AI)
**072: PII** ← 071 (Data Privacy)
**073: Sensitive Data** ← 071 (Data Privacy)

### Non-Profit Branch
**095: Stakeholder** ← 091 (501c3), 092 (Mission)
**098: Grant** ← 091 (501c3)
**101: Operating Budget** ← 091 (501c3)
**102: Program Services** ← 092 (Mission)

### Ethics Foundation
**051: AI Ethics** ← 001 (AI)
**058: Discrimination** ← 051 (AI Ethics)

---

## TIER 3: INTERMEDIATE CONCEPTS
These concepts require Tier 1 and/or Tier 2 knowledge.

### ML Techniques
**003: Deep Learning** ← 002 (ML), 006 (Neural Network)
**006: Neural Network** ← 002 (ML), 007 (Algorithm)
**008: Training Data** ← 002 (ML)
**009: Model** ← 002 (ML), 007 (Algorithm)
**010: Supervised Learning** ← 002 (ML), 008 (Training Data)
**011: Unsupervised Learning** ← 002 (ML), 008 (Training Data)
**012: Reinforcement Learning** ← 002 (ML)

### ML Tasks
**013: Classification** ← 010 (Supervised Learning)
**014: Regression** ← 010 (Supervised Learning)
**015: Clustering** ← 011 (Unsupervised Learning)
**016: Feature** ← 009 (Model), 008 (Training Data)
**017: Prediction** ← 009 (Model), 002 (ML)
**018: Inference** ← 009 (Model), 017 (Prediction)

### LLM Basics
**032: Large Language Model** ← 031 (Generative AI), 004 (NLP)
**033: GPT** ← 032 (LLM)
**034: Prompt** ← 032 (LLM)
**036: Token** ← 032 (LLM), 004 (NLP)

### Ethics Expansion
**052: Algorithmic Bias** ← 051 (AI Ethics), 009 (Model)
**053: Dataset Bias** ← 052 (Algorithmic Bias), 008 (Training Data)
**062: Black Box** ← 009 (Model), 051 (AI Ethics)
**066: Digital Divide** ← 051 (AI Ethics)

### Privacy Regulations
**077: GDPR** ← 071 (Data Privacy), 072 (PII)
**078: CCPA** ← 071 (Data Privacy), 072 (PII)
**083: Consent** ← 071 (Data Privacy)
**085: Data Breach** ← 071 (Data Privacy)

### Non-Profit Operations
**093: Theory of Change** ← 092 (Mission), 102 (Program Services)
**103: Administrative Costs** ← 101 (Operating Budget)
**104: Fundraising Costs** ← 101 (Operating Budget)
**106: Capacity Building** ← 092 (Mission)
**108: Volunteer Management** ← 095 (Stakeholder)
**109: Board of Directors** ← 091 (501c3), 095 (Stakeholder)

---

## TIER 4: APPLIED CONCEPTS
These concepts require foundational and intermediate knowledge.

### Advanced ML
**019: Overfitting** ← 009 (Model), 008 (Training Data)
**020: Underfitting** ← 009 (Model), 008 (Training Data)
**021: Accuracy** ← 017 (Prediction), 013 (Classification)
**022: Precision** ← 013 (Classification), 017 (Prediction)
**023: Recall** ← 013 (Classification), 017 (Prediction)
**027: Hyperparameter** ← 009 (Model), 002 (ML)
**028: Optimization** ← 027 (Hyperparameter), 009 (Model)
**029: Gradient Descent** ← 028 (Optimization), 007 (Algorithm)

### Advanced LLM
**035: Prompt Engineering** ← 034 (Prompt), 032 (LLM)
**037: Context Window** ← 036 (Token), 032 (LLM)
**038: Temperature** ← 032 (LLM), 035 (Prompt Engineering)
**043: Embeddings** ← 032 (LLM), 016 (Feature)
**044: Transformer Architecture** ← 032 (LLM), 006 (Neural Network)
**045: Attention Mechanism** ← 044 (Transformer), 006 (Neural Network)
**046: Hallucination** ← 032 (LLM), 035 (Prompt Engineering)

### Advanced Ethics
**054: Selection Bias** ← 053 (Dataset Bias), 008 (Training Data)
**055: Confirmation Bias** ← 053 (Dataset Bias)
**056: Fairness** ← 052 (Algorithmic Bias), 051 (AI Ethics)
**057: Equity** ← 056 (Fairness), 051 (AI Ethics)
**059: Transparency** ← 051 (AI Ethics), 062 (Black Box)
**060: Explainability** ← 059 (Transparency), 009 (Model)
**061: Accountability** ← 051 (AI Ethics), 060 (Explainability)
**063: Interpretability** ← 060 (Explainability), 009 (Model)

### Privacy Operations
**074: Data Anonymization** ← 072 (PII), 071 (Data Privacy)
**075: De-identification** ← 074 (Anonymization), 072 (PII)
**076: Data Minimization** ← 071 (Data Privacy), 077 (GDPR)
**081: Data Controller** ← 071 (Data Privacy), 077 (GDPR)
**082: Data Processor** ← 081 (Data Controller), 077 (GDPR)
**084: Opt-in/Opt-out** ← 083 (Consent), 071 (Data Privacy)
**086: Encryption** ← 071 (Data Privacy), 085 (Data Breach)
**087: Access Control** ← 071 (Data Privacy), 086 (Encryption)
**088: Data Retention** ← 071 (Data Privacy), 077 (GDPR)

### Fundraising Tools
**111: Donor Management System** ← 097 (Donor), 001 (AI)
**112: CRM** ← 111 (DMS), 095 (Stakeholder)
**114: Donor Segmentation** ← 097 (Donor), 015 (Clustering)
**120: Personalized Outreach** ← 097 (Donor), 114 (Segmentation)
**121: Email Optimization** ← 120 (Personalized Outreach), 002 (ML)

### Program Tools
**126: Chatbot** ← 004 (NLP), 032 (LLM)
**127: Virtual Assistant** ← 126 (Chatbot), 001 (AI)
**133: Multilingual Translation** ← 004 (NLP), 032 (LLM)
**134: Transcription** ← 004 (NLP), 005 (Computer Vision)
**135: Closed Captioning** ← 134 (Transcription), 004 (NLP)

### Operations Tools
**146: Workflow Automation** ← 001 (AI), 007 (Algorithm)
**147: Document Processing** ← 004 (NLP), 005 (Computer Vision)
**148: Email Classification** ← 004 (NLP), 013 (Classification)
**149: Meeting Scheduling** ← 001 (AI), 146 (Workflow Automation)
**150: Expense Management** ← 146 (Workflow Automation), 147 (Document Processing)

### Content Creation
**166: Content Generation** ← 031 (Generative AI), 032 (LLM)
**167: Copywriting** ← 166 (Content Generation), 034 (Prompt)
**172: Image Generation** ← 031 (Generative AI), 005 (Computer Vision)
**180: Content Calendar** ← 166 (Content Generation), 146 (Workflow Automation)

---

## TIER 5: ANALYTICAL CONCEPTS
These concepts require mastery of applied concepts and enable analysis.

### Performance Metrics
**024: F1 Score** ← 022 (Precision), 023 (Recall)
**025: Confusion Matrix** ← 021 (Accuracy), 022 (Precision), 023 (Recall)
**026: ROC Curve** ← 025 (Confusion Matrix), 021 (Accuracy)
**030: Cross-Validation** ← 021 (Accuracy), 008 (Training Data)

### Advanced Gen AI
**039: Fine-tuning** ← 032 (LLM), 008 (Training Data), 040 (Transfer Learning)
**040: Transfer Learning** ← 002 (ML), 009 (Model)
**041: Zero-shot Learning** ← 032 (LLM), 035 (Prompt Engineering)
**042: Few-shot Learning** ← 041 (Zero-shot), 035 (Prompt Engineering)
**047: Grounding** ← 046 (Hallucination), 048 (RAG)
**048: RAG** ← 032 (LLM), 043 (Embeddings)
**049: Multimodal AI** ← 004 (NLP), 005 (Computer Vision), 032 (LLM)
**050: AI Agent** ← 049 (Multimodal), 032 (LLM), 007 (Algorithm)

### Advanced Ethics
**064: Algorithmic Auditing** ← 052 (Algorithmic Bias), 056 (Fairness), 060 (Explainability)
**065: Disparate Impact** ← 056 (Fairness), 058 (Discrimination)
**067: Informed Consent** ← 083 (Consent), 060 (Explainability)
**068: Beneficence** ← 051 (AI Ethics), 061 (Accountability)
**069: Non-maleficence** ← 068 (Beneficence), 051 (AI Ethics)
**070: Justice** ← 056 (Fairness), 057 (Equity), 069 (Non-maleficence)

### Advanced Privacy
**079: Right to Explanation** ← 060 (Explainability), 077 (GDPR)
**080: Data Subject** ← 077 (GDPR), 072 (PII)
**089: Right to be Forgotten** ← 077 (GDPR), 088 (Data Retention)
**090: Privacy by Design** ← 071 (Data Privacy), 076 (Data Minimization), 086 (Encryption)

### Non-Profit Strategy
**094: Impact Measurement** ← 093 (Theory of Change), 102 (Program Services)
**105: Sustainability** ← 101 (Operating Budget), 094 (Impact Measurement)
**107: Community Engagement** ← 096 (Beneficiary), 095 (Stakeholder)
**110: Strategic Plan** ← 092 (Mission), 093 (Theory of Change), 109 (Board)

### Advanced Fundraising
**113: Predictive Giving** ← 112 (CRM), 017 (Prediction), 114 (Segmentation)
**115: Major Gift Identification** ← 113 (Predictive Giving), 114 (Segmentation)
**116: Wealth Screening** ← 113 (Predictive Giving), 097 (Donor)
**117: Donor Retention** ← 112 (CRM), 113 (Predictive Giving)
**118: Lapsed Donor Reactivation** ← 117 (Donor Retention), 114 (Segmentation)
**119: Donor Lifetime Value** ← 113 (Predictive Giving), 117 (Donor Retention)
**122: Subject Line Generation** ← 121 (Email Optimization), 031 (Generative AI)
**123: Grant Writing Assistance** ← 098 (Grant), 166 (Content Generation)
**124: Foundation Matching** ← 098 (Grant), 013 (Classification)
**125: Campaign Performance Analysis** ← 121 (Email Optimization), 094 (Impact Measurement)

### Advanced Program Delivery
**128: Service Recommendation** ← 127 (Virtual Assistant), 013 (Classification)
**129: Needs Assessment** ← 128 (Service Recommendation), 096 (Beneficiary)
**130: Sentiment Analysis** ← 004 (NLP), 013 (Classification)
**131: Social Listening** ← 130 (Sentiment Analysis), 004 (NLP)
**132: Content Personalization** ← 120 (Personalized Outreach), 114 (Segmentation)
**136: Accessibility Enhancement** ← 133 (Translation), 135 (Captioning)
**137: Community Dashboard** ← 094 (Impact Measurement), 157 (Data Visualization)
**138: Outreach Optimization** ← 017 (Prediction), 130 (Sentiment Analysis)
**141: Case Management** ← 129 (Needs Assessment), 112 (CRM)
**142: Referral Matching** ← 128 (Service Recommendation), 141 (Case Management)
**143: Feedback Analysis** ← 130 (Sentiment Analysis), 004 (NLP)
**144: Attendance Tracking** ← 146 (Workflow Automation), 147 (Document Processing)

### Advanced Operations
**151: Invoice Processing** ← 147 (Document Processing), 150 (Expense Management)
**152: Inventory Management** ← 017 (Prediction), 146 (Workflow Automation)
**153: Space Utilization** ← 152 (Inventory), 017 (Prediction)
**154: Staff Scheduling** ← 028 (Optimization), 146 (Workflow Automation)
**155: Time Tracking** ← 146 (Workflow Automation), 154 (Staff Scheduling)
**156: Report Generation** ← 146 (Workflow Automation), 166 (Content Generation)
**157: Data Visualization** ← 156 (Report Generation), 094 (Impact Measurement)
**158: Budget Forecasting** ← 017 (Prediction), 101 (Operating Budget)
**160: Compliance Monitoring** ← 077 (GDPR), 146 (Workflow Automation)
**161: Contract Analysis** ← 004 (NLP), 147 (Document Processing)
**162: Vendor Management** ← 112 (CRM), 161 (Contract Analysis)
**163: Asset Tracking** ← 152 (Inventory), 146 (Workflow Automation)
**164: Cybersecurity** ← 085 (Data Breach), 086 (Encryption), 087 (Access Control)
**165: Backup Automation** ← 146 (Workflow Automation), 088 (Data Retention)

### Advanced Content
**168: Social Media Post Creation** ← 166 (Content Generation), 167 (Copywriting)
**169: Blog Writing** ← 166 (Content Generation), 167 (Copywriting)
**170: Newsletter Creation** ← 169 (Blog Writing), 121 (Email Optimization)
**171: Press Release Writing** ← 167 (Copywriting), 166 (Content Generation)
**173: Video Creation** ← 172 (Image Generation), 005 (Computer Vision)
**174: Podcast Editing** ← 134 (Transcription), 004 (NLP)
**175: Infographic Design** ← 172 (Image Generation), 157 (Data Visualization)
**176: Template Customization** ← 166 (Content Generation), 132 (Personalization)
**177: Brand Voice Consistency** ← 167 (Copywriting), 166 (Content Generation)
**178: Content Optimization** ← 166 (Content Generation), 130 (Sentiment Analysis)
**179: A/B Testing** ← 178 (Content Optimization), 030 (Cross-Validation)

---

## TIER 6: STRATEGIC & EVALUATIVE CONCEPTS
These highest-level concepts require mastery of most prior concepts.

### Risk & Evaluation
**139: Impact Forecasting** ← 094 (Impact Measurement), 017 (Prediction), 093 (Theory of Change)
**140: Waitlist Management** ← 028 (Optimization), 129 (Needs Assessment)
**145: Outcome Measurement** ← 094 (Impact Measurement), 139 (Impact Forecasting)
**159: Risk Assessment** ← 017 (Prediction), 028 (Optimization), 164 (Cybersecurity)

### Implementation Strategy
**181: Digital Transformation** ← 001 (AI), 110 (Strategic Plan), 106 (Capacity Building)
**182: Change Management** ← 181 (Digital Transformation), 095 (Stakeholder)
**183: Technology Adoption** ← 182 (Change Management), 181 (Digital Transformation)
**184: ROI** ← 094 (Impact Measurement), 185 (TCO)
**185: Total Cost of Ownership** ← 101 (Operating Budget), 190 (SaaS)
**186: Scalability** ← 009 (Model), 189 (Cloud)
**187: Integration** ← 188 (API), 190 (SaaS), 112 (CRM)
**188: API** ← 001 (AI), 189 (Cloud)
**191: Vendor Lock-in** ← 185 (TCO), 190 (SaaS)
**192: Pilot Program** ← 183 (Technology Adoption), 193 (Proof of Concept)
**193: Proof of Concept** ← 183 (Technology Adoption)
**194: MVP** ← 193 (Proof of Concept), 195 (Iterative Development)
**195: Iterative Development** ← 192 (Pilot), 194 (MVP)
**196: User Acceptance Testing** ← 194 (MVP), 183 (Technology Adoption)
**197: Training Program** ← 182 (Change Management), 183 (Technology Adoption)
**198: Knowledge Base** ← 197 (Training), 166 (Content Generation)
**199: Technical Debt** ← 185 (TCO), 195 (Iterative Development)

### Governance (Highest Level)
**200: Governance Framework** ← 051 (AI Ethics), 061 (Accountability), 090 (Privacy by Design), 110 (Strategic Plan), 182 (Change Management)

---

## Learning Pathway Recommendations

### Fast Track (Essentials Only - 60 concepts)
Tier 1 → Select Tier 2 → Core Tier 4 applications → Key Tier 5 analytics

### Standard Track (Comprehensive - 120 concepts)
Tier 1 → Complete Tier 2 → Complete Tier 3 → Most of Tier 4 → Selected Tier 5

### Advanced Track (Complete - 200 concepts)
All Tiers in sequence with deep dives into Tier 5 and Tier 6

### Role-Based Tracks

**Executive Director Track:**
Focus on: Strategy concepts (181-200), Ethics (51-70), Non-Profit fundamentals (91-110), High-level fundraising (113-119)

**Program Manager Track:**
Focus on: Program delivery (126-145), Content creation (166-180), Community engagement, Impact measurement

**Development Director Track:**
Focus on: Fundraising tools (111-125), CRM, Email optimization, Grant writing, Donor analytics

**Operations Manager Track:**
Focus on: Operations tools (146-165), Workflow automation, Document processing, Budget forecasting

**Technical Staff Track:**
Focus on: All AI foundations (1-50), Integration, APIs, Implementation concepts (181-200)

---

## Dependency Visualization Notes

This DAG can be visualized with:
- **Nodes:** Concepts (numbered circles/boxes)
- **Edges:** Prerequisites (arrows from prerequisite to dependent concept)
- **Colors:** By Bloom's level or category
- **Vertical Layers:** Tier levels
- **Horizontal Grouping:** By category

Suggested tool for visualization: D3.js, Graphviz, or Mermaid for web-based rendering.

---

**Document Version:** 1.0  
**Total Dependencies Mapped:** 800+ relationships
