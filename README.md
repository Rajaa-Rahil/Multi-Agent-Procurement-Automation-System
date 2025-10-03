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

  ### Requirements

- **Python 3.11** - Core programming language.
- **Jupyter Notebook/JupyterLab** - The environment of development and execution.
- **Dotenv** - For environment variables.
- **CrewAI** - Multi-agent framework for AI coordination.
- **Pydantic** - For structured output.
- **AI Agents** - Specialized autonomous asgents for different tasks.
- **Web APIs** - SerperDev for web search, ScrapeGraph AI for web scraping.
- **HTML and Bootstrap** - Professional report generation and styling.

### Agent Architecture

**1. Search Queries Recommendation Agent**
**Role:** Generates varied search queries involving brands, types, and technologies.
**Output:** Structured search queries targeting specific e-commerce sites.

**2. Search Engine Agent**
**Role:** Executes web searches using generated queries.
**Tools:** SerperDevTool for comprehensive web searching.
**Output:** Filtered search results with confidence scoring and relevance analysis.

**3. Web Scraping Agent**
**Role:** Extracts detailed product information from e-commerce pages.
**Tools:** Custom web scraping tool using ScrapeGraph AI.
**Output:** Structured product data with prices, specifications, and features.

**4. Procurement Report Author Agent**
**Role:** Generates professional HTML procurement reports with analysis and recommendations.
**Output:** Bootstrap-styled HTML report with executive summary and insights.


### Installation and Setup

1. Download the repository.
2. Install the required Python packages.
3. Create a `.env` file in the root directory to store your API keys:
```python
   OPENAI_API_KEY=your_openai_api_key
   SERPER_API_KEY=your_serper_api_key
   SGAI_API_KEY=your_scrapegraph_ai_api_key
   AGENTOPS_API_KEY=your_agentops_api_key
```
4. Open the Jupyter Notebook and set your model.
5. Customize the search parameters and then run the cells:

### Output Files

The project generates foure files:

- `step_1_suggested_search_queries.json` – Suggested search queries. 
- `step_2_search_results.json` – Curated search results.  
- `step_3_extracted_products.json` – Extracted product details with analysis.
- `step_4_procurement_report.html` - Professional procurement report.

###  Acknowledgments

- Built with [CrewAI](https://www.crewai.com). 
- Uses [OpenAI](https://openai.com) models.  
- Search powered by [Serper](https://serper.dev).



