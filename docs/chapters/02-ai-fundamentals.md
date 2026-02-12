# Chapter 2: AI Fundamentals - Core Concepts

Understanding how AI actually works under the hood.

---

## Learning Objectives

By the end of this chapter, you will be able to:

- **Explain** the difference between AI, machine learning, and deep learning
- **Understand** supervised, unsupervised, and reinforcement learning
- **Describe** how neural networks process information
- **Identify** key AI terminology and concepts
- **Recognize** different types of AI models and their applications

**Bloom's Level:** 2 (Understand) | **Time:** 3-4 hours

---

## 2.1 Machine Learning Explained

Machine Learning (ML) is a subset of AI where systems learn from data without being explicitly programmed for every scenario.

### The Traditional Programming vs. Machine Learning

**Traditional Programming:**
```
Rules + Data → Answers
```
You write explicit rules, give it data, and get answers.

**Machine Learning:**
```
Data + Answers → Rules
```
You give examples (data + correct answers), and the system learns the rules.

### Example: Email Spam Filter

**Traditional:** Write rules like "if email contains 'FREE MONEY', mark as spam"
- Problem: Spammers adapt, endless rule updates needed

**Machine Learning:** Show the system 10,000 spam emails and 10,000 legitimate emails
- System learns patterns automatically
- Adapts to new spam tactics

!!! tip "Non-Profit Application"
    Use ML to predict which donors are likely to give again, which volunteers might drop out, or which programs will have the most impact.

---

## 2.2 Types of Machine Learning

### Supervised Learning

**Definition:** Learning from labeled examples (data with correct answers).

**How it works:**
1. Provide training data with labels (input → correct output)
2. Model learns patterns
3. Model predicts labels for new, unseen data

**Examples:**
- **Email classification:** Spam or not spam
- **Donor prediction:** Will give or won't give
- **Image recognition:** This is a cat, this is a dog

**Non-Profit Use Cases:**
- Predict donor retention
- Classify grant applications
- Identify at-risk program participants

---

### Unsupervised Learning

**Definition:** Finding patterns in data without labels.

**How it works:**
1. Provide unlabeled data
2. Model finds hidden patterns and groups
3. Discovers structure you didn't know existed

**Examples:**
- **Customer segmentation:** Group similar donors together
- **Anomaly detection:** Find unusual spending patterns
- **Topic modeling:** Discover themes in survey responses

**Non-Profit Use Cases:**
- Segment donors for targeted campaigns
- Identify volunteer clusters (weekend warriors, skill specialists, etc.)
- Find patterns in program feedback

---

### Reinforcement Learning

**Definition:** Learning through trial and error with rewards.

**How it works:**
1. Agent takes actions in an environment
2. Receives rewards (positive) or penalties (negative)
3. Learns to maximize rewards over time

**Examples:**
- Game playing (Chess, Go)
- Robotics
- Resource allocation optimization

**Non-Profit Use Cases:**
- Optimize email send times
- Resource allocation across programs
- Dynamic pricing for fundraising events

---

## 2.3 Neural Networks and Deep Learning

### What is a Neural Network?

A neural network is a computing system inspired by biological brains. It consists of:

- **Input layer:** Receives data
- **Hidden layers:** Process information
- **Output layer:** Produces results

### Simple Analogy

Think of a neural network like a series of filters:

```
Raw data → Filter 1 → Filter 2 → Filter 3 → Decision
```

Each filter extracts increasingly complex features.

**Example - Photo recognition:**
- Layer 1: Detects edges
- Layer 2: Detects shapes
- Layer 3: Detects objects
- Output: "This is a person"

### Deep Learning

**Definition:** Neural networks with many hidden layers (hence "deep").

**Why it matters:** Deep networks can learn very complex patterns that traditional ML can't.

**Applications:**
- Language translation
- Image generation
- Voice recognition
- Self-driving cars

**Non-Profit Applications:**
- Multilingual content translation
- Image classification for visual archives
- Voice-to-text for accessibility

---

## 2.4 Natural Language Processing (NLP)

NLP is AI's ability to understand and generate human language.

### Key NLP Tasks

| Task | Description | Non-Profit Example |
|------|-------------|-------------------|
| **Text Classification** | Categorize text | Sort donor emails by intent |
| **Sentiment Analysis** | Detect emotion | Analyze program feedback |
| **Translation** | Convert languages | Translate materials for AAPI communities |
| **Named Entity Recognition** | Identify names, places | Extract donor info from emails |
| **Text Generation** | Create new text | Draft thank-you letters |
| **Question Answering** | Answer queries | Chatbot for volunteer questions |

### How NLP Works

1. **Tokenization:** Break text into words/pieces
2. **Embedding:** Convert words to numbers
3. **Processing:** Neural network analyzes patterns
4. **Output:** Classification, generation, or translation

---

## 2.5 Computer Vision

Computer vision is AI's ability to interpret and understand visual information.

### Key Vision Tasks

| Task | Description | Non-Profit Example |
|------|-------------|-------------------|
| **Image Classification** | What's in this image? | Categorize event photos |
| **Object Detection** | Where are objects? | Count people at events |
| **Face Recognition** | Who is this? | Event check-in systems |
| **OCR** | Extract text from images | Digitize paper records |
| **Image Generation** | Create images | Generate social media graphics |

### Applications for Non-Profits

- Automated photo tagging for archives
- Attendance tracking at events
- Document digitization
- Accessibility features (image descriptions)

---

## 2.6 How AI Models Learn from Data

### The Training Process

1. **Collect Data:** Gather examples (more is better)
2. **Prepare Data:** Clean, organize, label
3. **Split Data:** 
   - Training set (80%): Teach the model
   - Validation set (10%): Tune the model
   - Test set (10%): Final evaluation
4. **Train Model:** Feed training data, adjust parameters
5. **Evaluate:** Test on unseen data
6. **Deploy:** Use in real world
7. **Monitor:** Track performance, retrain as needed

### Example: Donor Retention Model

```
1. Collect: 5 years of donor data
2. Prepare: Clean addresses, categorize giving levels
3. Split: 80% train, 10% validate, 10% test
4. Train: Model learns patterns of repeat donors
5. Evaluate: 85% accuracy on test set
6. Deploy: Score current donors for retention risk
7. Monitor: Retrain quarterly with new data
```

---

## 2.7 Key AI Terminology

### Model Performance Metrics

**Accuracy:** Percentage of correct predictions
```
Accuracy = Correct Predictions / Total Predictions
```

**Precision:** Of items marked positive, how many are actually positive?
```
Precision = True Positives / (True Positives + False Positives)
```

**Recall:** Of actual positive items, how many did we find?
```
Recall = True Positives / (True Positives + False Negatives)
```

**F1 Score:** Balance of precision and recall
```
F1 = 2 × (Precision × Recall) / (Precision + Recall)
```

### When to Use Each Metric

- **Accuracy:** Balanced datasets, general performance
- **Precision:** When false positives are costly (spam detection)
- **Recall:** When false negatives are costly (disease detection)
- **F1:** When you need balance between precision and recall

---

## 2.8 Common AI Challenges

### Overfitting

**Problem:** Model memorizes training data instead of learning patterns.

**Signs:**
- Perfect training performance
- Poor performance on new data

**Solutions:**
- Use more training data
- Simplify the model
- Use regularization techniques

### Underfitting

**Problem:** Model is too simple to capture patterns.

**Signs:**
- Poor training performance
- Poor test performance

**Solutions:**
- Use more complex model
- Add more features
- Train longer

### Data Quality Issues

**Problem:** Garbage in, garbage out.

**Common Issues:**
- Missing data
- Incorrect labels
- Biased sampling
- Outdated information

**Solutions:**
- Clean data thoroughly
- Validate labels
- Ensure representative sampling
- Update regularly

---

## Chapter Summary

- Machine Learning is AI that learns from data
- Three main types: Supervised, Unsupervised, Reinforcement
- Neural networks process information in layers
- Deep learning uses many layers for complex tasks
- NLP handles language, Computer Vision handles images
- Models learn through iterative training processes
- Performance metrics help evaluate model quality
- Common challenges: overfitting, underfitting, data quality

---

## Knowledge Check

1. What's the difference between supervised and unsupervised learning?
2. What is a neural network?
3. Give three examples of NLP tasks
4. What does "overfitting" mean?
5. Why is data quality important?

---

## Practical Exercise

**Scenario:** Your non-profit wants to predict which volunteers will return next month.

1. What type of ML would you use? (supervised/unsupervised/reinforcement)
2. What data would you need?
3. What would be your "features" (input variables)?
4. What would be your "label" (what you're predicting)?
5. How would you measure success?

---

[Next: Chapter 3 - Generative AI →](03-generative-ai.md)

[← Previous: Chapter 1](01-introduction.md) | [Chapter Index](index.md)
