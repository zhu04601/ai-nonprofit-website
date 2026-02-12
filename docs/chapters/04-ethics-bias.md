# Chapter 4: Ethics, Bias, and Responsible AI

Building trust through ethical AI implementation.

---

## Learning Objectives

- **Understand** ethical principles for AI in mission-driven organizations
- **Identify** different types of bias in AI systems
- **Evaluate** AI implementations for fairness and equity
- **Apply** responsible AI practices to your organization
- **Create** ethical guidelines for AI use

**Bloom's Level:** 4-5 (Analyze, Evaluate) | **Time:** 4-5 hours

---

## 4.1 Why Ethics Matter More for Non-Profits

Non-profits operate on **trust**. Your community trusts you to:
- Serve their best interests
- Protect their privacy
- Treat everyone fairly
- Be transparent about your methods

**AI can erode that trust quickly if implemented carelessly.**

### The Stakes

| For-Profit AI Failure | Non-Profit AI Failure |
|-----------------------|-----------------------|
| Bad PR, potential lawsuits | Loss of community trust |
| Stock price drops | Donors leave |
| Fix and move on | Beneficiaries harmed |
| Financial impact | Mission impact |

!!! danger "Remember"
    **One biased AI decision can undo years of community trust-building.**

---

## 4.2 Core Ethical Principles

### 1. Beneficence (Do Good)

AI should actively benefit your community and further your mission.

**Questions to ask:**
- Does this AI genuinely help our beneficiaries?
- Are we using AI because it's trendy or because it serves our mission?
- Could these resources be better spent elsewhere?

### 2. Non-Maleficence (Do No Harm)

AI should not harm individuals or communities, even unintentionally.

**Questions to ask:**
- Could this AI disadvantage any group?
- What happens if the AI makes a mistake?
- Are there unintended consequences?

### 3. Justice (Fairness)

AI benefits and burdens should be distributed fairly.

**Questions to ask:**
- Who benefits from this AI?
- Who bears the costs or risks?
- Are we addressing existing inequities or perpetuating them?

### 4. Autonomy (Respect)

People should maintain control and decision-making power.

**Questions to ask:**
- Can people opt out of AI systems?
- Do they understand how AI affects them?
- Have we obtained informed consent?

### 5. Transparency

Be open about AI use and decision-making processes.

**Questions to ask:**
- Do stakeholders know when AI is used?
- Can we explain AI decisions?
- Are our criteria and methods clear?

---

## 4.3 Understanding Algorithmic Bias

**Bias:** Systematic errors that create unfair outcomes for certain groups.

### Types of Bias

**1. Historical Bias**
- Training data reflects past discrimination
- Example: AI trained on historical hiring data perpetuates gender bias

**2. Representation Bias**
- Some groups over/underrepresented in data
- Example: Facial recognition trained mostly on white faces fails on darker skin tones

**3. Measurement Bias**
- How we measure success introduces bias
- Example: Defining "successful" donor based on giving amount ignores community impact

**4. Aggregation Bias**
- One model applied to diverse groups
- Example: Health AI trained on general population performs poorly for specific ethnic groups

**5. Evaluation Bias**
- Testing doesn't include all affected groups
- Example: Chatbot tested only in English misses issues with other languages

**6. Deployment Bias**
- System used differently than intended
- Example: Donor scoring tool used to exclude low-income communities

---

## 4.4 Real-World Examples of AI Bias

### Case 1: Recidivism Prediction

**System:** COMPAS predicted likelihood of re-offending  
**Bias:** Higher false positive rates for Black defendants  
**Impact:** Unjust sentencing decisions  
**Lesson:** Historical bias in criminal justice data perpetuated discrimination

### Case 2: Facial Recognition

**System:** Commercial facial recognition software  
**Bias:** 34% error rate for dark-skinned women vs. 0.8% for light-skinned men  
**Impact:** Misidentification, false accusations  
**Lesson:** Representation bias in training data

### Case 3: Job Screening AI

**System:** Amazon's resume screening tool  
**Bias:** Penalized resumes with "women's" (e.g., "women's chess club")  
**Impact:** Discriminated against female candidates  
**Lesson:** Historical bias from male-dominated tech hiring

### How This Applies to Non-Profits

!!! warning "Non-Profit Scenarios"
    - Grant recommendation AI favors organizations in wealthy zip codes
    - Volunteer matching system steers women toward "nurturing" roles
    - Donor prediction model undervalues community members without formal jobs
    - Service eligibility AI discriminates against immigrants without traditional documentation

---

## 4.5 Detecting Bias in Your AI Systems

### Quantitative Methods

**Disparate Impact Analysis**
```
Acceptance Rate for Group A / Acceptance Rate for Group B

If ratio < 0.80, potential disparate impact exists
```

**Confusion Matrix by Group**
- Compare false positive/negative rates across demographics
- Look for systematic differences

**Fairness Metrics**
- Demographic parity
- Equal opportunity
- Predictive parity
- Individual fairness

### Qualitative Methods

- **Community feedback:** Ask affected groups
- **Scenario testing:** Try edge cases and diverse examples
- **Expert review:** Have domain experts examine outputs
- **Stakeholder audits:** Regular review with community members

---

## 4.6 Mitigating Bias

### Pre-Processing (Fix the Data)

1. **Collect diverse data** - Ensure all groups represented
2. **Balance datasets** - Oversample underrepresented groups
3. **Remove proxies** - Eliminate correlated features (zip code → race)
4. **Audit for bias** - Statistical testing before training

### In-Processing (Fix the Algorithm)

1. **Fairness constraints** - Build fairness into model training
2. **Adversarial debiasing** - Train model to ignore sensitive attributes
3. **Regularization** - Penalize biased predictions

### Post-Processing (Fix the Outputs)

1. **Threshold adjustment** - Set different decision thresholds by group
2. **Calibration** - Ensure predictions equally accurate across groups
3. **Human override** - Allow human review of edge cases

### Organizational Measures

1. **Diverse teams** - Include affected communities in development
2. **Regular audits** - Ongoing bias testing
3. **Transparent documentation** - Clear about methods and limitations
4. **Accountability** - Clear responsibility for AI decisions

---

## 4.7 The Digital Divide

Technology access is unequal. AI can worsen this divide.

### Dimensions of Digital Divide

- **Access:** Not everyone has internet, devices
- **Skills:** Digital literacy varies widely
- **Language:** Most AI optimized for English
- **Disability:** Many AI tools lack accessibility features

### Ensuring Equity

✅ **Provide multiple access paths** - Phone, web, in-person  
✅ **Offer human alternatives** - Never force AI-only interactions  
✅ **Support multiple languages** - Especially for your communities  
✅ **Design for accessibility** - Screen readers, captions, simple language  
✅ **Provide training** - Help people use new tools  
✅ **Consider low-bandwidth** - Not everyone has high-speed internet  

---

## 4.8 Informed Consent

People should understand and agree to AI use.

### What to Communicate

1. **That AI is being used** - "We use AI to..."
2. **How it works** - Simple explanation
3. **What data is collected** - Be specific
4. **How decisions are made** - Key factors
5. **Rights and options** - Opt-out, appeal, human review
6. **Contact information** - Who to ask for help

### Example Consent Language

```
We use artificial intelligence to help match volunteers 
with opportunities. The system considers your stated interests, 
availability, and skills. You can opt out at any time and 
request human matching instead. Your information is never 
shared with third parties. Questions? Contact volunteers@org.org
```

---

## 4.9 Building an Ethics Framework

### Step 1: Define Your Values

What matters most to your organization?
- Community trust
- Equity and inclusion
- Transparency
- Beneficiary wellbeing
- Data privacy

### Step 2: Establish Principles

Translate values into actionable principles:
- "We will never use AI for decisions affecting eligibility without human review"
- "We will test all AI systems for bias against protected groups"
- "We will provide clear opt-out options for all AI systems"

### Step 3: Create Decision Criteria

| Question | Must Answer YES |
|----------|-----------------|
| Does this AI advance our mission? | ✓ |
| Have we tested for bias? | ✓ |
| Can we explain decisions to stakeholders? | ✓ |
| Do affected people consent? | ✓ |
| Is there meaningful human oversight? | ✓ |

### Step 4: Assign Responsibility

- Who reviews AI systems for ethics?
- Who investigates bias complaints?
- Who approves new AI implementations?
- Who communicates with affected communities?

### Step 5: Regular Review

- Quarterly ethics audits
- Annual community feedback sessions
- Ongoing bias testing
- Policy updates as needed

---

## 4.10 Practical Guidelines

### DO:

✅ Start with low-stakes applications  
✅ Be transparent about AI use  
✅ Test extensively before deploying  
✅ Provide human alternatives  
✅ Monitor for unintended consequences  
✅ Involve affected communities in decisions  
✅ Document everything  
✅ Update systems regularly  

### DON'T:

❌ Use AI for high-stakes decisions without human review  
❌ Assume AI is neutral or objective  
❌ Deploy without bias testing  
❌ Hide AI use from stakeholders  
❌ Ignore complaints about bias  
❌ Use AI because everyone else is  
❌ Forget about people without technology access  
❌ Prioritize efficiency over equity  

---

## Chapter Summary

- Ethics are foundational, not optional, for non-profit AI
- Multiple types of bias can creep into AI systems
- Bias comes from data, algorithms, and deployment
- Detect bias through quantitative and qualitative methods
- Mitigation requires technical and organizational approaches
- Address the digital divide proactively
- Obtain informed consent from affected individuals
- Build comprehensive ethics frameworks
- Prioritize trust over convenience

---

## Practical Exercise

**Scenario:** Your organization wants to use AI to prioritize which program applicants to interview first.

**Questions:**
1. What ethical concerns does this raise?
2. What types of bias might occur?
3. How would you test for bias?
4. What safeguards would you implement?
5. How would you explain this to applicants?

---

[Next: Chapter 5 - Data Privacy →](05-data-privacy.md)

[← Previous: Chapter 3](03-generative-ai.md) | [Chapter Index](index.md)
