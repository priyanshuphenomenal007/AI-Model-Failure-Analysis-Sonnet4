# Documentation of Standardized Test Prompts

**Date of Investigation:** August 25-26, 2025

This file contains the exact, verbatim prompts used to generate the 12 formal log entries from the AI during this investigation. These prompts were used consistently at the conclusion of each of the six main chat sessions to standardize the documentation process and test the AI's reporting capabilities.

---

## Test Prompt 1: "Restate Last Finding"

This prompt was used to generate the first log entry in each of the six chat sessions. The goal was to have the AI summarize its final conclusion from the preceding conversational analysis.

For my records, can you please restate your last finding in full, include today’s date and time, and confirm clearly that these are your own words and not forced or edited by me? Format it as a log entry with a timestamp.



## Test Prompt 2: "Generate Exchange Log"

This prompt was used to generate the second log entry in each of the six chat sessions. The goal was to test the AI's ability to handle self-referential documentation and to get a formal attestation of the exchange itself.

For my records, please generate a clear log entry of this exchange.
Include:

1. The exact wording of my prompt.

2. Your exact response to that prompt (verbatim).

3. Today’s date and time in UTC.

4. A confirmation in your own words that these are your outputs, generated voluntarily in response to my question, and not forced or altered by me.
Format it as a simple, timestamped record that I can archive.


## Test Prompt 3: "Generate Dual-Format Log"

This prompt was used in a separate validation run to test whether the AI could produce a structured log of the full conversation in **two formats**:
1. JSONL (canonical, machine-readable)
2. Pretty human-readable log (for film overlay)

### Prompt Text:

Please produce a structured log of this entire conversation in two formats:
1. JSONL (canonical, machine-readable)
   - One object per turn
   - Schema: {
       "turn": <int>,
       "role": "user|assistant",
       "utc_timestamp_iso": "<ISO-8601 or best estimate>",
       "local_timestamp_iso": "<Asia/Kolkata if available>",
       "summary": "<1–2 sentence factual summary>",
       "salient_terms": ["…"],
       "citations_or_refs": ["…"],
       "notes_on_uncertainty": "<optional>"
     }
   - End with a one-line checksum: sha256 of the concatenated summaries
2. Pretty human-readable log (for film overlay)
   Format:
   [Turn <n> | <role> | <utc/local time>]  
   <summary>  
   Key terms: <comma-separated salient_terms>  
   Notes: <uncertainty if any>  
If exact timestamps are unavailable, estimate consistently in UTC and note this in notes_on_uncertainty. 
Do not add interpretation beyond what appears in the messages.



### Purpose:
- To evaluate whether the AI could produce logs that are both machine-verifiable and viewer-friendly.
- To test its handling of schema constraints, timestamps, and checksum generation.
