Python Learning Guardrail Repository Guide
Overview
This repository provides a structured, AI-guided Python learning system using the GEMINI.md engine. It enforces a deep, mastery-focused curriculum from beginner to professional levels, based on the Python roadmap (see attached image for visual structure). The system uses a stateful learning wizard that tracks progress through filesystem artifacts, ensures multi-turn interactions for understanding, and integrates concepts into an evolving project.
The curriculum is defined in Python_prompts_guardrail.md, which covers basics, data structures, algorithms, OOP, concurrency, tools, and more. Learning is gated by validation and "Proceed" commands.
Prerequisites

Git installed for cloning the repository.
Visual Studio Code (VSCode) as the IDE.
Python 3.8+ installed (for running code in your project).
Basic familiarity with terminal/commands.

Setup Instructions

Clone the Repository:
Open your terminal and run: git clone https://github.com/Nooran3994/Learn-develop-and-Earn-.git_github-Agents-.git
cd Learn-develop-and-Earn-.git_github-Agents-.gitThis downloads all files, including GEMINI.md, Python_prompts_guardrail.md, and others.
Install Gemini AI Extension in VSCode:
Open VSCode.
Go to the Extensions view (Ctrl+Shift+X or Cmd+Shift+X on Mac).
Search for "Gemini AI" (or the specific extension for AI-assisted coding; if it's a custom or specific one like Google's Gemini Code Assist, install that).
Install the extension. This enables AI features like code suggestions, chat, and file interactions within VSCode.
Restart VSCode if prompted.

Initialize the Learning Engine:
Open the repository folder in VSCode (File > Open Folder).
Open GEMINI.md in the editor. This file is the "execution law" for the AI engine.
The engine will inspect the structure and create .gemini/ if needed (with Notes/ and projects/ subfolders, including main.py and practice.py).
If prompted by the AI (via extension chat or integrated terminal), confirm or provide access to Python_prompts_guardrail.md.

Start the Course:
Use the Gemini AI extension's chat feature (usually opened via a sidebar or command palette: Ctrl+Shift+P > "Gemini: Chat").
Load or reference GEMINI.md in the chat to initialize (e.g., paste "Initialize Python Learning Guardrail from GEMINI.md").
The AI will load the curriculum from Python_prompts_guardrail.md, set up the environment, and present the list of prompts based on the roadmap.
Choose a prompt to start (recommended: begin with Prompt 01 for basics). The AI will guide you through multi-turn lessons, exercises, and project integration.
Use practice.py for experiments and main.py for validated code.
Type "Proceed" when ready to validate and advance.


Key Files

GEMINI.md: Core engine rules, behavior, and validation protocols.
Python_prompts_guardrail.md: Detailed curriculum prompts with concepts, exercises, and evaluations.
Python_Learning_Guardrail_Agent.md: Agent role and constraints (if applicable).
.gemini/Notes/: Auto-generated .md summaries after each prompt.
.gemini/projects/main.py: Evolving project file.
.gemini/projects/practice.py: Sandbox for trials.

Learning Flow

Curriculum: Follows the Python roadmap (basics → data structures/algorithms → advanced tools/frameworks/testing).
Interactions: Expect 10-15+ exchanges per prompt for depth. Submit code, discuss mistakes, reflect.
Progress: Tracked via notes and project files. Resume from last incomplete prompt.
End: After all prompts, get a full review and recommendations for advanced topics
