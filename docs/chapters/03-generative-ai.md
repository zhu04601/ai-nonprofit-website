# Chapter 3: Generative AI and Large Language Models

Understanding the AI revolution powered by models that create content.

---

## Learning Objectives

- **Explain** what generative AI is and how it differs from traditional AI
- **Understand** how large language models (LLMs) work
- **Apply** prompt engineering techniques effectively
- **Recognize** capabilities and limitations of LLMs
- **Use** generative AI tools for non-profit applications

**Bloom's Level:** 2-3 (Understand, Apply) | **Time:** 3-4 hours

---

## 3.1 What is Generative AI?

**Generative AI** creates new content—text, images, audio, video—based on patterns learned from training data.

### Traditional AI vs. Generative AI

| Traditional AI | Generative AI |
|----------------|---------------|
| Classifies existing data | Creates new content |
| "Is this spam?" | "Write an email" |
| "What's in this image?" | "Generate an image" |
| Analyzes patterns | Produces original outputs |

### Real-World Applications

- **Text:** Write emails, articles, reports, social media posts
- **Images:** Create graphics, illustrations, photos
- **Code:** Generate software programs
- **Audio:** Compose music, generate voices
- **Video:** Create animations, edit videos

---

## 3.2 Large Language Models (LLMs)

LLMs are AI models trained on vast amounts of text to understand and generate human language.

### Popular LLMs

- **ChatGPT** (OpenAI) - General purpose, widely used
- **Claude** (Anthropic) - Focused on safety, helpful for analysis
- **Gemini** (Google) - Integrated with Google services
- **Llama** (Meta) - Open source option

### How LLMs Work

1. **Training:** Learn patterns from billions of web pages, books, articles
2. **Tokenization:** Break text into small pieces (tokens)
3. **Prediction:** Predict next most likely token based on context
4. **Generation:** String predictions together to form coherent text

### LLM Capabilities

✅ Writing and editing  
✅ Translation  
✅ Summarization  
✅ Question answering  
✅ Code generation  
✅ Data analysis  
✅ Creative brainstorming  
✅ Formatting and organizing  

---

## 3.3 The Art of Prompting

A **prompt** is your instruction to an AI model. Good prompts get good results.

### Basic Prompt Structure

```
[Context] + [Task] + [Format] + [Constraints]
```

**Example:**
```
Context: You are a fundraising expert for non-profits.
Task: Write a donor thank-you email.
Format: Keep it under 200 words, warm and personal.
Constraints: Mention the $500 gift supported youth programs.
```

### Prompt Engineering Tips

!!! tip "Effective Prompts"
    1. **Be Specific** - "Write a 100-word email" not "write an email"
    2. **Give Context** - Explain who you are, what you need
    3. **Provide Examples** - Show the style/format you want
    4. **Iterate** - Refine based on outputs
    5. **Use Roles** - "Act as a grant writing expert..."

### Common Prompt Patterns

**Few-Shot Learning:**
```
Example 1: [input] → [output]
Example 2: [input] → [output]
Now do: [your input]
```

**Chain of Thought:**
```
Let's think step-by-step:
1. First, analyze...
2. Then, consider...
3. Finally, conclude...
```

**Template Filling:**
```
Fill in this template:
Subject: [catchy subject line]
Body: [personalized greeting]
...
```

---

## 3.4 Practical Applications for Non-Profits

### Content Creation

**Use Case:** Draft social media posts

**Prompt:**
```
Create 5 Facebook posts promoting our youth coding workshop.
Audience: Parents in AAPI communities.
Tone: Encouraging, culturally aware.
Include: Date (March 15), Free registration, Skills learned.
```

### Email Communications

**Use Case:** Donor thank-you emails

**Prompt:**
```
Write a warm thank-you email to a first-time donor who gave $50.
Mention: Their gift helps provide art supplies to 10 children.
Tone: Grateful but not overly formal.
Length: 150 words.
Include: Invitation to visit our center.
```

### Grant Writing

**Use Case:** Draft program descriptions

**Prompt:**
```
Write a 250-word program description for a grant proposal.
Program: Multimedia education for refugee youth
Key points: Builds tech skills, cultural expression, career pathways
Include: Outcomes, who we serve, why it matters
```

### Translation

**Use Case:** Multilingual outreach

**Prompt:**
```
Translate this volunteer recruitment flyer into:
1. Spanish
2. Vietnamese  
3. Hmong

Maintain the warm, welcoming tone.
Adapt idioms if direct translation doesn't work.
```

---

## 3.5 Understanding Tokens and Context Windows

### What are Tokens?

Tokens are chunks of text that LLMs process. Roughly:
- 1 token ≈ 0.75 words (English)
- "Hello world" = 2 tokens
- "Artificial intelligence" = 2 tokens

### Context Window

The **context window** is how much text an LLM can "remember" at once.

| Model | Context Window |
|-------|----------------|
| GPT-3.5 | ~4,000 tokens (~3,000 words) |
| GPT-4 | ~8,000-32,000 tokens |
| Claude | ~100,000 tokens (~75,000 words) |
| Gemini | ~1 million tokens |

**Why it matters:** 
- Larger context = Can process longer documents
- Can "remember" entire conversations
- Better for analyzing complex materials

---

## 3.6 Temperature and Other Parameters

### Temperature

Controls randomness in outputs:

- **0.0** - Deterministic, predictable (good for factual tasks)
- **0.7** - Balanced creativity and consistency
- **1.0+** - Very creative, less predictable (good for brainstorming)

**Example:**
```
Temperature 0.0: "Thank you for your generous donation."
Temperature 1.0: "Your incredible generosity fills our hearts with gratitude!"
```

### Other Parameters

- **Max Tokens:** Limit response length
- **Top-P:** Alternative to temperature
- **Frequency Penalty:** Avoid repetition
- **Presence Penalty:** Encourage new topics

---

## 3.7 LLM Limitations and Hallucinations

### What LLMs Can't Do (Well)

❌ Real-time information (unless connected to search)  
❌ Complex math (without tools)  
❌ Accessing private/proprietary data  
❌ Perfect accuracy on all facts  
❌ Understanding visual content (unless multimodal)  

### Hallucinations

**Definition:** When an LLM confidently generates false information.

**Why it happens:**
- LLMs predict plausible text, not truth
- No fact-checking mechanism
- Trained on internet data (including misinformation)

**How to minimize:**
1. Ask for sources/citations
2. Verify critical information
3. Use retrieval-augmented generation (RAG)
4. Be specific: "Only use information from [source]"
5. Cross-check with multiple queries

!!! warning "Critical Rule"
    Never use LLM outputs for high-stakes decisions without human verification!

---

## 3.8 Advanced Techniques

### Retrieval-Augmented Generation (RAG)

Combine LLM with your own data:

1. Store your documents in a database
2. When user asks a question, retrieve relevant docs
3. Feed docs + question to LLM
4. LLM answers based on YOUR data

**Non-Profit Use:** Answer questions about your specific programs using only your documentation.

### Fine-Tuning

Train an LLM on your specific data to specialize it.

**When to consider:**
- You have lots of domain-specific data
- Generic LLMs don't capture your organization's voice
- Need consistent brand messaging

**Cost:** Usually expensive; start with good prompting first.

### Function Calling

Let LLMs trigger specific actions:

```
User: "Email our top 10 donors about the gala"
→ LLM extracts: action=send_email, recipients=top_10_donors, content=gala_invite
→ Your system executes the action
```

---

## 3.9 Ethical Considerations

### Bias in LLMs

LLMs reflect biases in training data:
- Cultural stereotypes
- Gender bias
- Racial bias
- Socioeconomic assumptions

**Mitigation:**
- Review outputs for bias
- Test with diverse perspectives
- Have humans review before publishing
- Provide diverse examples in prompts

### Privacy Concerns

!!! danger "Never Input"
    - Personal identifiable information (PII)
    - Private donor data
    - Confidential organizational information
    - Sensitive beneficiary information

Most LLM providers use inputs for training (unless you have specific agreements).

### Copyright and Attribution

- LLM outputs may resemble copyrighted material
- Always review and edit generated content
- Add your own insights and analysis
- Cite sources when appropriate

---

## 3.10 Getting Started: Practical Steps

### Week 1: Explore

1. Sign up for ChatGPT, Claude, or Gemini (free tiers)
2. Try 10 different prompts
3. Compare outputs from different models
4. Document what works well

### Week 2: Apply to Your Work

1. Draft 5 donor emails
2. Create 10 social media posts
3. Translate 1 flyer to 3 languages
4. Summarize 3 meeting notes

### Week 3: Develop Best Practices

1. Create prompt templates for common tasks
2. Document your best prompts
3. Share with team
4. Collect feedback

### Week 4: Scale

1. Integrate into workflows
2. Train staff on effective prompting
3. Measure time saved
4. Identify next use cases

---

## Chapter Summary

- Generative AI creates new content from patterns
- LLMs are trained on vast text data
- Effective prompting is key to good results
- Understand tokens, context windows, and parameters
- Watch for hallucinations and verify outputs
- Apply ethically with awareness of bias and privacy
- Start small, iterate, and scale gradually

---

## Knowledge Check

1. What's the difference between traditional AI and generative AI?
2. What is a prompt and why does it matter?
3. What is a "hallucination" in LLMs?
4. List 3 practical applications for non-profits
5. What data should you never input to public LLMs?

---

## Practical Exercise

**Challenge:** Create 3 donor thank-you emails using an LLM

**Requirements:**
- Different donation amounts ($25, $100, $500)
- Personal, warm tone
- Mention specific program impact
- Under 150 words each
- Unique content (not repetitive)

**Bonus:** Translate one email into 2 languages

---

[Next: Chapter 4 - Ethics & Bias →](04-ethics-bias.md)

[← Previous: Chapter 2](02-ai-fundamentals.md) | [Chapter Index](index.md)
