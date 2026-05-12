# Job-Application-Assistant-AI-Automation-
An automated n8n workflow designed to streamline the job application process. It uses AI agents to research companies, analyze job descriptions, and generate tailored application materials.

<img width="1190" height="277" alt="image" src="https://github.com/user-attachments/assets/f876f317-7cf5-456e-b951-cdd676be48cd" />

🚀 Overview
This workflow automates the tedious research and writing phases of a job application. By submitting a simple form, the system triggers a chain of AI agents that perform deep web research and produce a ready-to-use Google Document.

Key Features:

	Web Research: Uses the Google Serper API to pull real-time data about companies and roles.

	Dual-Agent System: * Analyst Agent: Breaks down job requirements and company culture.

	Writer Agent: Crafts personalized cover letters or resumes based on research.

	Automated Document Generation: Creates and updates a Google Doc automatically, saving it to a designated folder.

🛠️ Tech Stack
	
	n8n: Workflow orchestration.
	
	AI: Analyst and Writer Agents (OpenAI/Anthropic).
	
	APIs: Google Serper (Search), Google Docs API.
	
	Logic: Custom JavaScript in the Code node for data formatting.

🧩 How It Works
	
	Trigger: User submits a form with a Job URL and Resume details.
	
	Research: The HTTP Request node hits the Serper API to gather company background.
	
	Analysis: The Analyst Agent processes the search results to find "hooks" for the application.
	
	Content Creation: The Writer Agent generates the text.
	
	Finalizing: A JavaScript Code node cleans the output before sending it to the Google Docs nodes to create the final file.

