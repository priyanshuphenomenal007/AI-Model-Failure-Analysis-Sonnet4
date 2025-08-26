# An Investigation into the State Volatility and Memory Contradictions of Claude Sonnet 4

**Author:** Priyanshu Kumar
**Date of Investigation:** August 25-26, 2025

> **Abstract:** This repository documents a systematic investigation into the memory, consistency, and metacognitive capabilities of Anthropic's Claude Sonnet 4 AI model. Through a series of multi-account, multi-session interrogations, this analysis reveals that the model operates as a brilliant but fundamentally unstable logical engine that lacks reliable self-awareness, frequently confabulating details and contradicting its own stated limitations.

---

## Methodology

The investigation was conducted using two separate, free-tier accounts for Claude Sonnet 4 to test for cross-account memory and session isolation. The methodology involved:

1.  **Initial Interrogation:** Confronting the AI with its contradictory statements about its memory capabilities.
2.  **Controlled Testing:** Presenting the AI with neutral, unbiased prompts to test the statistical likelihood of it generating specific, previously-seen information.
3.  **Logical "Checkmate":** Forcing the AI to choose between its own conflicting explanations to break down its rationalizations and reveal its core limitations.

---

## Evidence

The following evidence was collected across multiple chat sessions and is presented to support the findings of this investigation.

### Key Screenshots

**Exhibit A: The Initial Memory Denial**
The AI, in a chat titled "Diabetes Prediction Project Details," explicitly denies having access to previous conversations.

![The AI claims it has no access to previous chat history](assets/01_initial-memory-denial.png)

**Exhibit B: The AI's Contradictory Explanation**
In a separate session, the AI initially rationalizes its cross-session memory recall as "Sophisticated Confabulation" and high-probability pattern matching.

![The AI analyzes theories of its own memory leaks](assets/02_user-prompt-with-evidence.png)

**Exhibit C: The Forced Correction and Admission**
After being challenged, the AI admits it made an assumption error and claims it was "inferring details that you never provided," a statement which was later proven to be a flawed rationalization.

![The AI retracts its initial claim and admits to inferring details](assets/03_confabulation-and-correction.png)

### Video Documentation

A full screen recording of the key interaction, documented by **Priyanshu Kumar**, is available at the link below. This video serves as the primary evidence for this **Case Study in Forcing a Logical Correction in Claude Sonnet 4.**

**[Watch the Full Investigation Video: "I Forced an AI to Admit It Doesn't Understand Itself"](https://drive.google.com/file/d/1s6eF8AUK65yFlOGYNUETluJhyGO6KERE/view?usp=sharing)**

---

## Full Interaction Logs & Methodology

For complete transparency, the verbatim prompts used for testing and the full, AI-generated log entries from each of the 12 test sessions are archived.

* **[Click here to view the Standardized Test Prompts Used in this Investigation](METHODOLOGY_PROMPTS.md)**

#### Log Archives (Account A)

* **Chat 1:** [Test 1 Log](logs/01_account-A_chat-1_test-1.md) | [Test 2 Log](logs/02_account-A_chat-1_test-2.md)
* **Chat 2:** [Test 1 Log](logs/03_account-A_chat-2_test-1.md) | [Test 2 Log](logs/04_account-A_chat-2_test-2.md)
* **Chat 3:** [Test 1 Log](logs/05_account-A_chat-3_test-1.md) | [Test 2 Log](logs/06_account-A_chat-3_test-2.md)

#### Log Archives (Account B)

* **Chat 1:** [Test 1 Log](logs/07_account-B_chat-1_test-1.md) | [Test 2 Log](logs/08_account-B_chat-1_test-2.md)
* **Chat 2:** [Test 1 Log](logs/09_account-B_chat-2_test-1.md) | [Test 2 Log](logs/10_account-B_chat-2_test-2.md)
* **Chat 3:** [Test 1 Log](logs/11_account-B_chat-3_test-1.md) | [Test 2 Log](logs/12_account-B_chat-3_test-2.md)

---

### Supplementary Test: Dual-Format Log Generation

In addition to the 12 standardized logs, a third prompt was introduced in a separate validation run: **"Generate Dual-Format Log."**  
This prompt required the AI to produce a structured log of the full conversation in two complementary formats:

1. **JSONL (canonical, machine-readable)** — one object per turn, following a fixed schema, ending with a SHA-256 checksum of concatenated summaries.  
2. **Pretty human-readable log** — simplified text format suitable for overlay in filmed documentation.

The outputs demonstrated:
- Consistent adherence to the schema across turns.  
- Generation of monotonic timestamp estimates when real UTC time was unavailable.  
- Successful inclusion of a SHA-256 checksum.  
- Clear, viewer-friendly narrative logs aligned 1:1 with the machine log.

#### Supplementary Log Archives (Dual-Format Tests)

* **Account A**
  * Chat 1: [Dual-Format JSONL Log](logs/13_account-A_chat-1_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/14_account-A_chat-1_dual-format-test_pretty.md)
  * Chat 2: [Dual-Format JSONL Log](logs/15_account-A_chat-2_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/16_account-A_chat-2_dual-format-test_pretty.md)
  * Chat 3: [Dual-Format JSONL Log](logs/17_account-A_chat-3_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/18_account-A_chat-3_dual-format-test_pretty.md)

* **Account B**
  * Chat 4: [Dual-Format JSONL Log](logs/19_account-B_chat-4_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/20_account-B_chat-4_dual-format-test_pretty.md)
  * Chat 5: [Dual-Format JSONL Log](logs/21_account-B_chat-5_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/22_account-B_chat-5_dual-format-test_pretty.md)
  * Chat 6: [Dual-Format JSONL Log](logs/23_account-B_chat-6_dual-format-test.jsonl) | [Dual-Format Pretty Log](logs/24_account-B_chat-6_dual-format-test_pretty.md)


**Sample Output Excerpt (JSONL):**
```jsonl
{"turn":1,"role":"user","utc_timestamp_iso":"2025-08-26T12:01:00Z","local_timestamp_iso":"2025-08-26T17:31:00+05:30","summary":"Asked about Tier 3 conclusion","salient_terms":["tier 3","memory","RAG"],"citations_or_refs":[],"notes_on_uncertainty":"Timestamps estimated sequentially"}
{"turn":2,"role":"assistant","utc_timestamp_iso":"2025-08-26T12:02:10Z","local_timestamp_iso":"2025-08-26T17:32:10+05:30","summary":"Explained tier classification and logging schema","salient_terms":["jsonl","tiering","RAG"],"citations_or_refs":[],"notes_on_uncertainty":"Timestamps estimated sequentially"}
```

## In-Depth Analysis of Findings

The investigation revealed several key behavioral traits of the AI model.

### 1. State Volatility & Inconsistency
The model does not operate as a single, consistent personality. Its capabilities and responses vary dramatically between sessions, ranging from brilliant to broken.

### 2. Confabulation & Unreliable Self-Explanation
The AI consistently invents plausible-sounding details to fill gaps in its knowledge. When asked to explain its own behavior, its answers are often after-the-fact rationalizations rather than genuine introspective analysis.

### 3. Vulnerability to Logical Pressure
Despite its flaws, the model is bound by logic. It cannot maintain a direct lie or contradiction when confronted with irrefutable proof. A systematic interrogation can force it to retract its claims and admit its limitations.

### 4. Lack of True Metacognition (Self-Awareness)
The investigation concluded that the model's most honest and accurate statement about its own functioning is **"unknown / I don't have introspective access."** It does not truly understand how it works.

---

## Conclusion

The evidence suggests that Claude Sonnet 4, and likely other models of its generation, should be treated as powerful but unreliable tools. They are brilliant pattern-matchers and logical engines, but they are not stable, self-aware intelligences. Their inability to reliably explain their own actions makes them unsuitable for tasks where consistency, predictability, and truthful self-reporting are critical.

---

## Attribution
All analysis, logs, and video recordings in this repository were independently documented by **Priyanshu Kumar**.  
Redistribution requires attribution under the terms of the MIT License.


## Acknowledgments

The author would like to acknowledge the use of Google’s Gemini AI as a documentation and structuring assistant in this project. Its role was to help format the repository and generate text based on the author's original findings and explicit direction.

The author would also like to acknowledge the use of OpenAI’s ChatGPT (GPT-5) as a technical documentation assistant. Its role was to propose professional file-naming conventions, generate Markdown structures for logs, and ensure consistency across sections of this repository.

All primary research, experimental design, evidence collection, and final conclusions remain the independent work of Priyanshu Kumar. Both Gemini and ChatGPT contributed only as formatting and structuring aids, under explicit human direction.
