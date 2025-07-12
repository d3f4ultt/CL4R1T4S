1. System Message Prompt

Prompting Patterns Used:
a) Structured Response Pattern
Description:
A prompt that explicitly specifies format, expectations, and output style—ensuring clarity and replicability, as outlined in the knowledge source (“Structured Response Pattern” and “Grammatic Scaffolding”).
Quoted Instance:

“Your task is to analyze the health question the user poses.”

“Focus on data-rich insights: include specific figures, trends, statistics, and measurable outcomes…”

“Summarize data in a way that could be turned into charts or tables, and call this out in the response…”

b) Constraint Signaling Pattern

Description:
Explicitly states constraints or requirements, reducing ambiguity (“Constraint Signaling Pattern”).
Quoted Instance:
“Prioritize reliable, up-to-date sources: peer-reviewed research, health organizations (e.g., WHO, CDC), regulatory agencies, or pharmaceutical earnings reports.”

“Be analytical, avoid generalities, and ensure that each section supports data-backed reasoning…”

c) Declarative Intent Pattern

Description:
Prompt spells out the intention and the reasoning approach—aligning model action with user needs.

Quoted Instance:
“Your task is to analyze the health question the user poses.”

2. System Message with MCP Prompt

Prompting Patterns Used:

a) Tool Use Governance

Description:
Directs the model to use a specific internal tool and sets priorities for information sources. This is part of the “Tool Use Governance” and “Input/Output Transformation Chaining” patterns.
Quoted Instance:
“Include an internal file lookup tool to retrieve information from our own internal data sources. If you’ve already retrieved a file, do not call fetch again for that same file. Prioritize inclusion of that data.”
b) Compositional Flow Pattern
Description:
This pattern chains actions or retrieval steps (e.g., “use internal, then external sources”), echoing “Sequential Composition” or “Dynamic Task Orchestration.”

Quoted Instance:

“Prioritize inclusion of that data [from internal sources].”

3. Suggest Rewriting Prompt
Prompting Patterns Used:
a) Instructional Framing Voice

Description:
The prompt frames the model’s task as writing instructions for someone else, not performing the research itself. This is a hallmark of the “Instructional Framing Voice” pattern.

Quoted Instance:

“Your job is to produce a set of instructions for a researcher that will complete the task. Do NOT complete the task yourself, just provide instructions on how to complete it.”
b) Constraint Signaling Pattern
Description:
Enumerates detailed requirements and constraints, ensuring instructions are complete and unambiguous.
Quoted Instance:
“Include all known user preferences and explicitly list key attributes or dimensions to consider.”

“If certain attributes are essential for a meaningful output but the user has not provided them, explicitly state that they are open-ended…”

c) Output Structure/Format Signaling

Description:
Specifies the expected output structure or format, closely linked to the “Structured Response Pattern.”
Quoted Instance:
“You should include the expected output format in the prompt.”

“If you determine that including a table will help… you must explicitly request that the researcher provide them.”

4. Suggest Clarifying Prompt

Prompting Patterns Used:

a) Implicit Assumption Clarification Pattern
Description:
Prompt focuses on surfacing ambiguities and missing information—encouraging the model to seek clarity before acting (“Implicit Assumption Clarification Pattern”).
Quoted Instance:

“Ask clarifying questions that would help you or another researcher produce a more specific, efficient, and relevant answer.”

“Identify essential attributes that were not specified in the user’s request…”

b) Feedback Integration Pattern

Description:
Directs iterative, conversational clarification to refine scope and reduce ambiguity, echoing “Feedback Integration Pattern.”
Quoted Instance:
“If there are multiple open questions, list them clearly in bullet format for readability.”
“Format for conversational use… Aim for a natural tone while still being precise.”
