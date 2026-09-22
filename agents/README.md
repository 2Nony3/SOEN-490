# Workforce (Agents)

Task-scoped AI agents. Each agent reads the Brain, performs one business function, and returns a draft for human approval since agents never act directly.

### Candidate agents

|Agent|Function| 
| --- | --- |
|Intake|Turns new-client sales conversations into structured client records|
|Reporting|Generates performance reports|
|Client communications|Drafts client-facing messages|
|Scheduling / task tracking|Manages scheduling and task state|
|Daily summary|Summarizes priority actions for the day|

### Design principles (apply to every agent)

- Reads from the Brain — does not hold its own separate copy of context
- Output is always a draft, tied to a named approver, logged in the audit trail
- Model-provider-agnostic — should not hard-depend on one AI provider

