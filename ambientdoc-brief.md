# AmbientDoc AI
_Physician Documentation Assistant - NorthBridge Health System_

Organization: NorthBridge Health System
Current Users: 3 physicians, live notes
Expansion Request: CMO scale to 40 physicians

## Background
NorthBridge Health System is a regional healthcare network with 12 hospitals and 200+ outpatient clinics across the Pacific Northwest. Like most health systems, they face a documentation crisis: physicians spend an average of two hours per day on clinical notes, pulling them away from patient care.

Eighteen months ago, NorthBridge's innovation team piloted AmbientDoc — an AI system that listens to physician-patient conversations and generates clinical notes automatically. The pilot launched quietly with three volunteer physicians in a single outpatient clinic in Portland.

The results looked promising. Physicians reported saving 45–60 minutes per day. Patient satisfaction scores in that clinic ticked up. The CMO heard about it at a leadership offsite and immediately flagged it as a priority initiative.

That was the moment things started to move faster than the operating system could handle.

## The Initiative - What It Is and How It Works
### What AmbientDoc does
AmbientDoc uses a voice-to-text AI model to transcribe physician-patient conversations in real time. A second model processes the transcript and generates a structured clinical note in SOAP format (Subjective, Objective, Assessment, Plan). The physician reviews the draft note, makes edits, and signs off before it enters the EHR.
The system is built on a third-party AI vendor — MedScribe Inc. — whose API NorthBridge calls through a middleware layer their engineering team built. The underlying language model is a fine-tuned clinical variant of a commercial base model.

NorthBridge does not control the underlying model. MedScribe Inc. can update it. NorthBridge engineering can update the middleware prompts. Either change can affect clinical output quality — and neither requires a formal review process under the current setup.

### The current state
The pilot has been running live for 14 months with the same three physicians.

## The Expansion Pressure
Three weeks ago, the CMO presented AmbientDoc at the system's quarterly board meeting. She cited the pilot's positive physician feedback and framed it as a competitive differentiator — two rival health systems are deploying similar tools. The board asked for a timeline.
The CMO told the board: 90 days to 40 physicians across four clinics.


