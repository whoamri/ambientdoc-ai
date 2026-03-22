You are scanning the AmbientDoc AI initiative against the AI-First
Operating System framework. Use available MCP tools to query:

1. LINEAR: Search project AMDOC for active epics. Extract:
   - Initiative name and description
   - Current stage (Explore/Prototype/Pilot/Production/Scale)
   - Named owner (person, not team)
   - Last updated date
   - Any gate criteria documented


2. GITHUB: Check repo ambientdoc-ai, branch main, last 30 days:
   - Any model version changes or prompt file edits
   - Whether a gate review was linked to any model change
   - Days since last eval run (look for /evals/ directory changes)


3. SLACK: Search #ambient-doc-feedback, last 14 days:
   - Any physician complaints or quality concerns
   - Volume of complaint signals (count unique users)
   - Whether any Slack thread generated a Jira ticket


Then apply the four-layer gap scan:
   THE MAP:    Is this initiative visible in a shared registry?
   THE OWNERS: Is there one named person accountable for
               behavioral outcomes (not deployment)?
   THE GATES:  Is there a written criterion for the next
               stage transition? Was it applied at last change?
   THE PULSE:  Is there a scheduled review? Are there event
               triggers? Did the Slack complaints trigger one?


Output a portfolio table row with six columns:
   Initiative | Stage | Owner | Next Gate | Risk Flag | Tier


For Risk Flag: HIGH if real users, clinical/financial/hiring
impact, or model changed without review. MEDIUM if vendor
dependency or no monitoring. LOW if internal, reversible,
limited exposure.


End with a one-paragraph Signal recommendation: what needs
to happen before this initiative can move to the next stage.