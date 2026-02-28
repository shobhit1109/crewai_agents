# CrewAI Agentic Workflows

This project demonstrates how to use the CrewAI framework to automate content creation and email assistance using autonomous agents. The workflows are implemented in Jupyter notebooks and leverage the CrewAI library to coordinate multiple specialized agents.

## Project Structure
- `crewai_agent_basic.ipynb`: Demonstrates a basic CrewAI agent setup, ideal for learning the fundamentals of agent creation and task execution.
- `crewai_research_write_QA.ipynb`: Shows an agentic workflow for content creation, with Researcher, Writer, and Reviewer agents.
- `crewai_email_agent.ipynb`: Features an Email Assistant agent for simplifying emails and replacing jargon.
- `requirements.txt`: List of required Python packages.

## Features
- **Basic Agent Example**: Learn CrewAI basics with a simple, single-agent workflow.
- **Content Creation Crew**: Automate research, writing, and review for educational content.
- **Email Jargon Assistant**: Rewrite emails by replacing technical jargon with simple language and suggestions.
- **End-to-End Automation**: From research to writing to review, and email simplification, the processes are fully automated.
- **Customizable**: Easily adapt agent roles, goals, and tasks for different content domains or communication needs.

## How It Works

### Basic Agent Crew
The `crewai_agent_basic.ipynb` notebook demonstrates how to set up and run a single CrewAI agent for a simple, focused task. This is ideal for users new to CrewAI who want to understand the core concepts of agent definition, task assignment, and execution without the complexity of multiple agents or tools.

### Content Creation Crew
1. **Researcher Agent**: Gathers and structures information on a given topic.
2. **Writer Agent**: Converts the research into a step-by-step guide with examples.
3. **Reviewer Agent**: Checks the guide for accuracy, clarity, and beginner-friendliness.
4. **Crew Coordination**: The CrewAI `Crew` object manages the sequence and collaboration of tasks.

### Email Assistant Crew
1. **Email Assistant Agent**: Analyzes a provided email, identifies technical jargon, and suggests replacements with simpler language.
2. **Custom Tool**: The agent uses a custom tool to map common corporate/technical terms to plain English and generates a list of suggestions.
3. **Crew Coordination**: The CrewAI `Crew` object manages the email simplification task.

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- OpenAI API Key (set as `OPENAI_API_KEY` in your environment)

### Installation
1. Clone this repository or download the project files.
2. (Recommended) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   # On Windows:
   .venv\Scripts\activate
   # On Unix/Mac:
   source .venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set your OpenAI API key in a `.env` file or as an environment variable:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```

### Usage

#### Basic Agent Crew
1. Open `crewai_agent_basic.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells to see a simple CrewAI agent perform its assigned task.

#### Content Creation Crew
1. Open `crewai_research_write_QA.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells to execute the agentic workflow.
3. The final output will be a reviewed, beginner-friendly guide on the chosen topic.

#### Email Assistant Crew
1. Open `crewai_email_agent.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells to see how the Email Assistant agent suggests jargon replacements and produces a simplified email.

## Customization
- **Change the Topic**: Modify the task descriptions in the content creation notebook to target a different subject.
- **Add/Remove Agents**: Define new agent roles or tasks as needed for your workflow.
- **Adjust Output Format**: Update the `expected_output` fields to change the structure of the generated content or email output.
- **Expand Jargon List**: Edit the custom tool in the email agent notebook to include more jargon or domain-specific terms.

## Example Output
- The basic agent notebook shows a single agent completing a straightforward task, ideal for learning CrewAI basics.
- The content creation notebook generates a structured, step-by-step guide with examples, reviewed for clarity and accuracy.
- The email agent notebook outputs a professional email with all jargons replaced by simple language and a list of suggestions for each jargon found.

## License
This project is for educational and demonstration purposes.

