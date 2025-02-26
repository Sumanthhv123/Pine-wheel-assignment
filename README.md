# Pine-wheel-assignment
This project implements an agentic cybersecurity workflow using LangGraph, designed to automate security assessments with controlled execution, task management, and report generation. The system integrates various security tools like Nmap, Gobuster, FFUF, and Sqlmap, enforcing scope constraints to prevent unauthorized scans.

**Overview**

This project implements an agentic cybersecurity workflow using LangGraph and LangChain to automate security tasks such as reconnaissance, scanning, and vulnerability assessment. The agent dynamically plans, executes, and adapts security tasks while enforcing scope constraints.

**Features**

Task Planning: Uses LLMs to break down high-level security instructions into executable steps.

Dynamic Execution: Executes security tools (e.g., nmap, gobuster, ffuf, sqlmap) and adapts based on results.

Scope Enforcement: Ensures all actions stay within allowed domains/IP ranges.

Error Handling & Retrying: Implements failure handling and retry logic for resilience.

Logging & Reporting: Logs execution details and generates security reports.

**Technologies Used**

Python

LangGraph & LangChain

OpenAI API (for task breakdown)

Streamlit (for UI deployment)

Security Tools: nmap, gobuster, ffuf, sqlmap

**Installation**

Prerequisites

Ensure you have the following installed:

Python 3.8+

pip install -r requirements.txt

Security tools (nmap, gobuster, ffuf, sqlmap) installed and in PATH

# Clone the repository
git clone https://github.com/your-repo/langgraph-cybersec-agent.git
cd langgraph-cybersec-agent

# Install dependencies
pip install -r requirements.txt

Usage

Running the Cybersecurity Agent
python agent.py

Running with Streamlit UI
streamlit run ui.py

Workflow

Define Scope: Users specify allowed domains/IP ranges.

Plan Tasks: The agent breaks down instructions into actionable tasks.

Execute Tasks: Tasks are executed while enforcing scope constraints.

Handle Errors & Retry: Tasks are retried if they fail.

Generate Reports: A security report is created summarizing results.

**File Structure**

langgraph-cybersec-agent/
│── agent.py            # Main agent logic & LangGraph workflow
│── tools.py            # Wrappers for security tools (nmap, ffuf, etc.)
│── task_manager.py     # Task management & scheduling
│── scope.py            # Scope enforcement logic
│── logger.py           # Logging execution details
│── report.py           # Report generation module
│── ui.py               # Streamlit-based UI
│── requirements.txt    # Python dependencies
│── README.md           # Project documentation

**Future Improvements**

Add more security tools and integrations.

Implement advanced result parsing for deeper automation.

Introduce AI-driven attack path simulations.

License

MIT License

Contributing

Contributions are welcome! Open an issue or submit a pull request.

Contact

For any questions or feedback, reach out via GitHub Issues.
