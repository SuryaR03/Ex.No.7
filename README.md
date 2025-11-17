# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

# Date: 17-11-2025
# Register no. 212223110056 
# Aim: To develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.

# Explanation: 

## Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."


Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.

## Core Requirements of the Personal Productivity Assistant

| Feature                 | Description                                                      |
| ----------------------- | ---------------------------------------------------------------- |
| **Task Management**     | Add tasks naturally, support deadlines, priorities, summaries.   |
| **Smart Scheduling**    | Schedule events, detect conflicts, suggest alternate time slots. |
| **Wellness Tips**       | Provide hydration reminders, posture tips, breathing exercises.  |
| **General Queries**     | Natural conversational responses to general questions.           |
| **Adaptation**          | Learns preferred tone, work hours, snooze habits.                |
| **Memory Simulation**   | Stores user preferences to tailor future responses.              |
| **Natural Interaction** | Understands everyday language without fixed commands.            |

## System Design Overview
## Architecture Components
Input Module – Receives user’s natural language commands.
Intent Analyzer – Determines if input is a task, event, wellness, preference, etc.
Action Handler – Performs the requested action.
Memory Store – Saves preferences like tone or work hours.
LLM Response Generator – Produces smooth conversational replies.
Feedback Loop – Updates behaviour when preferences change.

## Prompt Templates
## System Prompt
“You are a supportive and efficient Personal Productivity Assistant. Respond clearly and naturally.”
Task
User: {task_input}
Assistant: Extracts task info → generates structured task.
Scheduler
User: {event_input}
Assistant: Parses the time → checks conflicts → schedules event.
Wellness
User context: {mood_input}
Assistant: Provides a targeted wellness suggestion.
General Query
User: {question}
Assistant: Gives a concise helpful answer

## Simulation Workflow
## Example Inputs

“Add assignment submission on Friday at 6 PM.”
“Schedule team call tomorrow at 3 PM.”
“I am feeling tired.”
“Change tone to formal.”
Model Response Process
Input →
Intent classification →
Action execution →
Memory update →
Natural reply generation

## Output (Simulated)
## Task Manager

User: Add assignment submission on Friday at 6 PM
Assistant: ✔ Added "Assignment submission" for Friday, 6 PM. Want an early reminder?
Smart Scheduler
User: Schedule team call tomorrow at 3 PM
Assistant: Scheduled “Team call” at 3 PM for 1 hour. No conflicts detected.
Wellness Support
User: I’m tired
Assistant: Try a quick 1-minute breathing break. Want me to begin? (Start/Later)
Preference Update
User: Change tone to formal
Assistant: Understood. I will respond more formally.
Adaptive Behaviour
User: Delay posture reminders
Assistant: Sure. I’ll reduce posture reminders and space them out more

## Memory Example
```
{
  "preferences": {
    "tone": "formal",
    "work_hours": {"start": "09:00", "end": "17:00"},
    "wellness_snooze": {"posture": 2}
  }
}
```
## Smart Scheduler
```
User: Schedule meeting with Priya tomorrow at 3 PM  
Assistant: Scheduled "Meeting with Priya" at 3 PM for 1 hour.
```

## Wellness Suggestion
```
User: I'm feeling stressed  
Assistant: Try a 2-minute guided breathing exercise. Shall I start a session now? (Start/Snooze)

```

## Preference Update
```
User: Set work hours 10:00–18:00  
Assistant: Work hours updated to 10:00–18:00.

```

## Adaptive Response
```
User: Use concise tone  
Assistant: Got it — I'll keep responses concise.

```

# Adaptation Mechanism:

Maintains a JSON-based memory with fields like:
```
{
  "preferences": {
    "preferred_tone": "concise",
    "work_hours": {"start": "10:00", "end": "18:00"},
    "snooze_counts": {"stretch": 3}
  }
}
```
If a wellness tip is repeatedly snoozed, the assistant delays its frequency.

Tone changes immediately affect all future responses.

## Output Summary

| Component           | Behaviour                                          |
| ------------------- | -------------------------------------------------- |
| **Task Manager**    | Manages tasks with deadlines and summaries.        |
| **Scheduler**       | Handles events and conflict detection.             |
| **Wellness System** | Gives timely health suggestions.                   |
| **Adaptive System** | Learns preferences and adjusts behaviour.          |
| **LLM Interaction** | Smooth, conversational natural language responses. |


# Result: 
The lab exercise resulted in the creation of a prototype concept for a personal assistant powered by large language models. Students were able to:
 Understand how to tailor LLM prompts to real-life applications.
 Foster creativity by designing features suited to their personal or academic lives.
 Learn prompt engineering techniques for optimal interaction with AI tools.
 Experience the versatility and utility of generative AI in solving everyday problems.
