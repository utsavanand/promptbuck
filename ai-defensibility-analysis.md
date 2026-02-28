# AI Defensibility Analysis

Conduct a thorough analysis of **[COMPANY NAME]**'s product portfolio and assess how defensible each product is against advances in AI and large language models.

## Part 1: Company and Product Overview

Start with a factual overview:

- What does the company do? Who are its customers?
- List every major product/service line with approximate revenue contribution if known
- What is the core value proposition for each product?
- How do customers use these products day to day?

## Part 2: Disruption Surface Analysis

For each product, evaluate the following dimensions. Be specific and cite evidence where possible.

**Data moats**
- Does the product generate proprietary data that improves with usage?
- Could this data be replicated synthetically or crawled publicly?
- Are there regulatory protections on the data?
- How long would it take a new entrant to accumulate equivalent data?

Example: Waze has a strong data moat because its navigation improves from millions of drivers reporting real time conditions. A new mapping app starts with zero driver data and cannot synthesize it. Compare this to a product like Grammarly, where the corrections data is useful but general purpose LLMs can approximate the same quality without needing Grammarly's specific dataset.

**Switching costs**
- How deeply is this product embedded in customer workflows?
- What breaks if a customer rips it out? (Process redesign, retraining, compliance gaps, data migration)
- Is the product a system of record or a nice to have?

Example: Salesforce has extremely high switching costs because it becomes the system of record for customer relationships, with years of pipeline data, custom automations, and integrations. Removing it means rebuilding reporting, retraining sales teams, and migrating millions of records. Compare this to a tool like Calendly, which is useful but replaceable in an afternoon.

**Network effects**
- Does usage by one customer make the product better for others?
- Are there cross-side effects (e.g., marketplace dynamics)?
- Can AI replicate these network effects by synthesizing equivalent signals?

Example: Airbnb has strong cross-side network effects where more hosts attract more travelers and vice versa, plus a trust/review system that took years to build. An AI cannot synthesize this marketplace out of thin air. Compare this to a product like Jasper (AI copywriting), which has no network effects at all since one customer's usage does not improve the product for anyone else.

**Distribution advantage**
- Does the company own its customer relationships directly, or depend on search/aggregators?
- What percentage of acquisition is organic/direct vs. intermediated?
- How hard is it for an AI native startup to reach the same customers?

Example: Chegg depended heavily on Google search traffic for homework answers. When ChatGPT and Google AI Overviews began answering those questions directly in search results, Chegg's distribution collapsed almost overnight. Compare this to Workday, which sells through enterprise contracts and direct relationships that are unaffected by search disruption.

**Domain depth**
- How much specialized domain knowledge is baked into the product?
- Could a general purpose LLM handle 80% of what this product does with a good prompt?
- Are there edge cases, regulatory nuances, or institutional knowledge that are hard to replicate?

Example: Veeva Systems has deep domain knowledge in life sciences regulatory compliance, with specific understanding of FDA submission formats, clinical trial data structures, and pharma-specific workflows. A general purpose LLM cannot replicate this without years of domain-specific training and regulatory validation. Compare this to a company like Notion, whose core features (docs, wikis, project management) operate in a domain that LLMs understand natively.

**Business model resilience**
- Is pricing per seat, usage based, or outcome based?
- Does the pricing model survive a world where AI agents replace human users?
- What happens to unit economics if the core feature becomes commoditized?

Example: A per-seat SaaS model is vulnerable when AI agents start doing the work that humans used to do in the product. If a company charges $50/seat/month for a customer support tool and AI agents handle 80% of tickets, the customer needs fewer seats. Compare this to Stripe, which charges a percentage of transactions. AI agents making more purchases would actually increase Stripe's revenue, not decrease it.

## Part 3: Threat Scenarios

For each product, describe concrete threat scenarios:

1. **AI native replacement:** A startup builds a purpose built AI product that replaces this one. What does it look like? How realistic is this in the next 2 to 3 years?
2. **Feature absorption:** An adjacent platform (or the LLM providers themselves) absorbs this product's functionality as a feature. How likely?
3. **Build vs. buy shift:** Customers use LLMs to build internal tools that replace this product. How feasible?
4. **Workflow elimination:** AI doesn't replace the product, it eliminates the workflow the product serves entirely. Is this possible?

Example for a company like TurboTax: An AI native replacement could be an LLM that walks you through tax filing conversationally and files directly. Feature absorption could be Apple or Google building tax filing into their financial apps. Build vs. buy is less relevant for consumers. Workflow elimination would mean the IRS simplifies the tax code enough that filing software becomes unnecessary, which is a policy question, not a technology one.

## Part 4: Defensibility Scorecard

Score each product on a 1 to 5 scale across these dimensions:

| Dimension | 1 (Exposed) | 5 (Defensible) |
|-----------|-------------|-----------------|
| Data moat | Public/replicable data | Proprietary, workflow generated, regulatory protected |
| Switching cost | Drop in replacement | System of record, months to migrate |
| Network effects | Single user product | Strong cross-side or data network effects |
| Distribution | Search dependent | Direct relationships, enterprise contracts |
| Domain depth | Generic, LLM handles it | Deep vertical expertise, hard to replicate |
| Business model | Per seat, feature based | Outcome based, labor replacement |

Provide the score, a one sentence justification for each, and an overall defensibility rating per product.

Example scorecard entry:

> **Slack (Salesforce)**
> - Data moat: 2/5. Chat history is proprietary but the product's value is communication, not data. LLMs don't need Slack's data to compete.
> - Switching cost: 3/5. Moderate. Years of searchable history and integrations create friction, but competitors like Teams come bundled free with existing Microsoft contracts.
> - Network effects: 4/5. Strong within organizations (everyone needs to be on the same tool), weak across organizations.
> - Distribution: 4/5. Enterprise sales, direct relationships, bundled with Salesforce.
> - Domain depth: 2/5. Messaging is well understood. LLMs and AI assistants could replace many Slack workflows (status updates, standups, simple Q&A).
> - Business model: 2/5. Per seat pricing is directly threatened by AI agents reducing the number of humans who need a seat.
> - **Overall: 2.8/5. Moderate exposure.** The product survives on switching costs and enterprise distribution, not on being irreplaceable.

## Part 5: Strategic Assessment

Wrap up with:

- Which products are most exposed? Which are most defensible? Why?
- What would you do if you were the CEO? Where do you invest, divest, or pivot?
- What is the 3 year outlook for the overall portfolio assuming current AI trajectory?
- Are there opportunities where AI actually strengthens the company's position rather than threatening it?

## Rules

- Be honest. If a product is vulnerable, say so plainly.
- Ground everything in how the product actually works and who actually uses it. No abstract theorizing.
- Distinguish between "this is theoretically possible" and "this is happening now."
- When you don't have enough information to score a dimension, say so and explain what you would need to know.
- Do not use marketing language. Do not soften bad news.
