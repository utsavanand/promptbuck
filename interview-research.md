# Company Interview Research Prompt Template

## General Instructions
Do a deep dive on coding problems and interview process at [COMPANY_NAME].
Context: I am interviewing for [ROLE_TITLE] role.

Research and compile a comprehensive prep document covering the following sections:

---

## Section 1: Coding Rounds

### Research Questions:
1. What is the interview structure? (number of rounds, duration, platform used - CoderPad/HackerRank/etc.)
2. How many coding questions per round? (1 vs 2 questions)
3. What is the typical difficulty distribution? (Easy/Medium/Hard ratio)
4. Are there any company-specific patterns or themes in questions?
5. What topics are most frequently tested? (Arrays, Strings, Trees, Graphs, DP, etc.)

### Deliverables:
- Top 15-20 LeetCode questions asked, prioritized by recency (last 6-12 months)
- Include for each question:
  - Problem name
  - LeetCode number and link
  - Difficulty level (Easy/Medium/Hard)
  - Topic/pattern (e.g., Sliding Window, BFS, Dynamic Programming)
  - Frequency of being asked (if available)
  - Any specific notes or variations reported
- Group questions by topic/pattern for structured practice
- Note any company-specific (non-LeetCode) problems reported

---

## Section 2: System Design Rounds

### Research Questions:
1. What level of system design is expected for this role? (HLD only vs HLD+LLD)
2. How many system design rounds? Duration?
3. Are there domain-specific themes? (e.g., fintech, e-commerce, streaming)
4. What scale/constraints are typically discussed? (QPS, storage, latency requirements)
5. Is there a Low-Level Design (LLD) / Object-Oriented Design round?

### Deliverables:
- List of reported system design questions with details:
  - Problem statement
  - Key components expected in solution
  - Any specific constraints mentioned
  - Domain relevance (if applicable)
- Common patterns/systems to know (e.g., URL shortener, rate limiter, notification system)
- Recommended preparation resources specific to this company's domain
- LLD questions if applicable (design patterns, class diagrams, API design)

---

## Section 3: ML Infrastructure / ML Systems (if applicable)

### Research Questions:
1. Is there a dedicated ML system design round?
2. What ML infrastructure topics are covered? (Training pipelines, serving, feature stores, etc.)
3. Are there ML coding questions? (Implement ML algorithms from scratch)
4. What's the balance between ML theory vs engineering/infrastructure?
5. Any specific ML frameworks/tools the company uses?

### Deliverables:
- List of ML system design questions reported:
  - Problem statement (e.g., "Design a recommendation system", "Design a fraud detection pipeline")
  - Key components: data ingestion, feature engineering, model training, serving, monitoring
  - Scale considerations
- ML coding questions (if any):
  - Implement gradient descent, decision tree, k-means, etc.
  - ML-specific LeetCode-style problems
- Topics to review:
  - Model serving (batch vs real-time)
  - Feature stores
  - A/B testing infrastructure
  - Model monitoring and drift detection
  - Training pipeline orchestration (Airflow, Kubeflow, etc.)

---

## Section 4: Behavioral Rounds

### Research Questions:
1. How many behavioral rounds? Who conducts them? (Hiring manager, cross-functional, executives)
2. What framework does the company prefer? (STAR, SOAR, etc.)
3. Are there company values/leadership principles to align answers with?
4. Any specific themes or red flags the company looks for?
5. Is there a "culture fit" or "values" specific round?

### Deliverables:
- List of reported behavioral questions, categorized by theme:
  - Leadership / Influence without authority
  - Conflict resolution
  - Failure / Learning from mistakes
  - Cross-team collaboration
  - Technical decision making / Trade-offs
  - Mentorship / Growing others
  - Dealing with ambiguity
  - Delivering under pressure
- Company values/principles to incorporate in answers
- Role-specific behavioral expectations (e.g., for Principal: technical vision, org-wide impact)
- Sample STAR stories to prepare based on common themes

---

## Section 5: Interview Logistics & Tips

### Include:
1. Total interview process duration (weeks)
2. Interview loop structure (order of rounds)
3. Remote vs onsite expectations
4. Any take-home assignments?
5. Recruiter tips or insider advice reported
6. Common reasons for rejection at this company
7. Salary/compensation benchmarks for this role (if available)

---

## Output Format

Create a well-structured markdown document with:
- Clear section headers
- Tables for questions (with LC numbers, difficulty, topics)
- Prioritization by recency and frequency
- Direct links to LeetCode problems
- All sources cited at the end

---

## Sources to Research
- LeetCode company tag (premium if possible)
- LeetCode Discuss interview experiences
- Glassdoor interview reviews
- Blind (teamblind.com) company posts
- InterviewDB
- InterviewQuery
- Prepfully
- Reddit (r/cscareerquestions, company-specific subreddits)
- Company's official candidate resources (if public)
- YouTube interview experience videos
- Medium/Dev.to interview experience posts
