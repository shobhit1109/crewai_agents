# CrewAI Content Creation Crew

This project demonstrates how to use the CrewAI framework to automate the process of researching, writing, and reviewing educational content using autonomous agents. The workflow is implemented in a Jupyter notebook and leverages the CrewAI library to coordinate multiple specialized agents.

## Features
- **Agentic Workflow**: Three agents (Researcher, Writer, Reviewer) collaborate to produce high-quality, beginner-friendly guides.
- **Modular Tasks**: Each agent is assigned a specific role and task, ensuring clarity and division of labor.
- **End-to-End Automation**: From research to writing to review, the process is fully automated.
- **Customizable**: Easily adapt agent roles, goals, and tasks for different content domains.

## Project Structure
- `crewai_research_write_QA.ipynb`: Main notebook demonstrating the agentic workflow for content creation.
- `requirements.txt`: List of required Python packages.

## How It Works
1. **Researcher Agent**: Gathers and structures information on a given topic.
2. **Writer Agent**: Converts the research into a step-by-step guide with examples.
3. **Reviewer Agent**: Checks the guide for accuracy, clarity, and beginner-friendliness.
4. **Crew Coordination**: The CrewAI `Crew` object manages the sequence and collaboration of tasks.

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
1. Open `crewai_research_write_QA.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells to execute the agentic workflow.
3. The final output will be a reviewed, beginner-friendly guide on the chosen topic.

## Customization
- **Change the Topic**: Modify the task descriptions in the notebook to target a different subject.
- **Add/Remove Agents**: Define new agent roles or tasks as needed for your workflow.
- **Adjust Output Format**: Update the `expected_output` fields to change the structure of the generated content.

## Example Output
The notebook will generate a structured, step-by-step guide with examples, reviewed for clarity and accuracy.

## License
This project is for educational and demonstration purposes.

## Acknowledgements
- [CrewAI](https://github.com/joaomdmoura/crewai) for the agentic workflow framework.
- OpenAI for language model APIs.
