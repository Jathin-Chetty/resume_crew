# Multi-Agent Job Application Optimization System

A sophisticated CrewAI-based system that uses specialized AI agents to optimize the entire job application process, from job research to interview preparation.

## 🚀 Problem Statement

Job applications are complex, multi-step processes requiring specialized expertise across different domains. Candidates must research job requirements, compile comprehensive profiles, tailor resumes to specific roles, and prepare for interviews - each requiring different skills and knowledge that most job seekers lack.

This system addresses these challenges by using AI agents that can process large amounts of information from multiple sources (job postings, GitHub profiles, personal data), apply specialized knowledge consistently, and provide personalized recommendations at scale.

### Our 4 Specialized Agents:

1. **Job Market Intelligence Analyst**: Scrapes and analyzes job postings to extract key requirements, skills, and qualifications
2. **Candidate Intelligence Specialist**: Compiles comprehensive candidate profiles from GitHub repositories and personal information
3. **Technical Resume Architect**: Tailors resumes to highlight relevant skills and experiences that match job requirements
4. **Technical Interview Coach**: Creates targeted interview questions and talking points based on the tailored resume and job requirements

## 🛠️ Tools Used

- **SerperDev**: Web search capabilities
- **ScrapeWebsite**: Job posting analysis
- **FileRead**: Resume processing
- **MDXSearch**: Semantic search of candidate data

## 📁 Project Structure

```
resume_crew/
├── test_notebook.ipynb    # Main Jupyter notebook with agent definitions
├── fake_resume.md         # Sample resume data for testing
├── utils.py              # Utility functions for API keys and formatting
└── README.md             # This file
```

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook
- OpenAI API key
- Serper API key

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Jathin-Chetty/resume_crew.git
cd resume_crew
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install crewai crewai-tools python-dotenv jupyter
```

4. Set up environment variables:
Create a `.env` file in the project root:
```
OPENAI_API_KEY=your_openai_api_key_here
SERPER_API_KEY=your_serper_api_key_here
```

5. Launch Jupyter Notebook:
```bash
jupyter notebook
```

6. Open `test_notebook.ipynb` and run the cells to start the multi-agent system.

## 💡 Usage

1. **Prepare your data**: Update the `fake_resume.md` file with your actual resume information
2. **Configure inputs**: Modify the `job_application_inputs` dictionary with your target job URL and GitHub profile
3. **Run the crew**: Execute the notebook cells to start the multi-agent analysis
4. **Review outputs**: Check the generated `tailored_resume.md` and `interview_materials.md` files

## 🔧 Configuration

The system is highly configurable. You can:

- Modify agent roles and backstories
- Adjust task descriptions and expected outputs
- Add new tools and data sources
- Customize the workflow and agent interactions

## 📊 Features

- **Comprehensive Job Analysis**: Deep extraction of job requirements and hidden qualifications
- **Professional Profile Building**: Analysis of GitHub activity, projects, and career history
- **ATS-Optimized Resume Tailoring**: Strategic alignment with job requirements
- **Interview Preparation**: Targeted questions and talking points
- **Context-Aware Processing**: Each agent builds upon previous agent outputs

## 🙏 Acknowledgments

- Built with [CrewAI](https://github.com/joaomdmoura/crewAI) framework
- Powered by OpenAI's GPT models
- Enhanced with SerperDev search capabilities
