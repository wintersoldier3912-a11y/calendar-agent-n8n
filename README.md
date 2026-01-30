# calendar-agent-n8n

📅 Calendar AI Agent using n8n
📌 Project Overview

This project implements a Calendar AI Agent using n8n that allows users to block time on their Google Calendar through natural language chat input.
The agent understands conversational requests like scheduling meetings and automatically creates calendar events using appropriate time slots.

The system is designed as a no-code / low-code AI automation workflow, focusing on logic, data flow, and AI-assisted understanding of user intent.

🎯 Objective

To design an AI-powered agent that:

Accepts scheduling requests via chat

Interprets natural language input

Extracts date, time, and event details

Blocks the corresponding time slot in Google Calendar

🛠️ Technology Stack

n8n – Workflow automation platform

Chat Node – Trigger for user interaction

AI / LLM Node – Natural language understanding and parsing

Google Calendar Node – Event creation and time-slot blocking

🔁 Workflow Description
Step 1: Chat Trigger

The workflow starts when a user sends a message via the Chat node.

Example input:

“Block my calendar for a meeting at 2 PM tomorrow”

Step 2: Natural Language Parsing

The AI agent analyzes the message and extracts:

Event title

Date

Start time

End time or duration

Additional notes (optional)

Relative time expressions such as today, tomorrow, or next Monday are supported.

Step 3: Time Slot Normalization

Parsed values are converted into structured date-time format.

If the end time is not specified, the system defaults to a 1-hour time slot.

Step 4: Google Calendar Integration

The structured event data is passed to the Google Calendar node.

A calendar event is created, effectively blocking the specified time slot.

Step 5: User Confirmation

The agent sends a confirmation message via chat showing:

Event name

Date

Time slot

In case of ambiguity, the agent asks for clarification.

✅ Supported Capabilities

Natural language scheduling

Relative and absolute time handling

Automatic time-slot blocking

Conversational confirmation

Error handling for unclear inputs

🧪 Sample Test Inputs

“Block my calendar for a meeting at 2 PM tomorrow”

“Schedule a call next Monday at 10 AM”

“Reserve 3 PM to 4 PM today for project discussion”

📄 Deliverables

n8n workflow design

AI prompt for natural language parsing

Google Calendar event mapping

Test case examples

This README documentation

ℹ️ Notes

This project focuses on workflow design and AI logic.

No code reading or implementation details are required, as per assignment instructions.

The solution demonstrates how AI and automation can be combined to solve real-world scheduling problems.
