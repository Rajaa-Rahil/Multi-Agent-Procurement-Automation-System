## Multi-Agent Procurement Automation

An intelligent AI-agents procurement automation system that utilizes CrewAI's multi-agent framework to automate product research, comparison, and reporting for business purchases.

### Overview

This project implements an automated procurement system using CrewAI's multi-agent framework. The system helps companies find the best products by automatically searching across multiple e-commerce platforms, extracting product details and specifications from various online stores, analyzing, comparing, and ranking findings to recommend the best options. It also generates professional HTML reports, summarizing results and procurement insights.

### Features

- **Multi-Agent Architecture:** Four AI agents each handle specific tasks and work together in a set order.
- **Smart Search Automation:** The system creates search queries and finds information online automatically.
- **Product Analysis:** Extract detailed specifications and compare products from multiple online stores.
- **Intelligent Ranking:** Uses AI to review and rank the best options by value.
- **Professional Reporting:** Automatically generate HTML report using Bootstrap style.
- **Price Comparison:** Comprehensive value-for-money analysis across multiple vendors.
- **Structured Data Processing:** Robust Pydantic models that keep all the information consistent and easy to work with.
- **Extensible Design:** This approach works great whethwer you are shopping for office supplies, industrial equipment, or anything else you need to source online.

  ### Technologies Used

- **Python 3.11** - Core programming language.
- **Jupyter Notebook/JupyterLab** - The environment of development and execution.
- **Dotenv** - For environment variables.
- **CrewAI** - Multi-agent framework for AI coordination.
- **Pydantic** - For structured output.
- **AI Agents** - Specialized autonomous asgents for different tasks.
- **Web APIs** - SerperDev for web search, ScrapeGraph AI for web scraping.
- **HTML and Bootstrap** - Professional report generation and styling.


### Installation and Setup

1. Download the repository.
2. Install the required Python packages.
3. Create a `.env` file in the root directory to store your API keys:
```python
   OPENAI_API_KEY=your_openai_api_key
   SERPER_API_KEY=your_serper_api_key
```
4. Open the Jupyter Notebook and set your model.
5. Customize the event details and then run the cells:

 ```python
event_details = {
    'event_topic': "Your Event Name",
    'event_city': "City, State",
    'tentative_date': "YYYY-MM-DD",
    'expected_participants': 100,
    'budget': 50000,
    'preferences': "your preferences here",
    'audience': "target audience description",
    'venue_type': "Venue Type"
}
```

### Output Files

The project generates three files:

- `venue_details.json` – Structured venue information. 
- `marketing_report.md` – Marketing strategy and outreach plan.  
- `risk_compliance_checklist.md` – Safety, risk assessmment and compliance chechlist.

###  Acknowledgments

- Built with [CrewAI](https://www.crewai.com). 
- Uses [OpenAI](https://openai.com) models.  
- Search powered by [Serper](https://serper.dev).



