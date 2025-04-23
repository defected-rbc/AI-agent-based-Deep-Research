# AI Agentic Research & Drafting System

A multi-agent AI system built with **LangGraph** and **LangChain** to automate deep research and answer drafting based on user queries.

## ✨ What It Does

This system orchestrates specialized AI agents to:

-   Analyze the user query and plan the research.
-   Coordinate and execute web searches using **Tavily**.
-   Fetch content from relevant web pages.
-   Synthesize information from search results and crawled content.
-   Draft a structured answer.
-   Review the draft and trigger revisions if needed.

## 🛠️ Technologies

-   **LangGraph:** Agent orchestration and workflow.
-   **LangChain:** Agent components, LLM/Tool integrations.
-   **Google Gemini API:** Primary LLM used for agent intelligence.
-   **Tavily API:** Web search capabilities.
-   **Requests & BeautifulSoup4:** Web content fetching and parsing.
-   **Python:** Core language.

## 🚀 Quick Setup

1.  **Install Libraries:**
    ```bash
    pip install -qU langchain langgraph langchain-community langchain-google-genai tavily-python requests beautifulsoup4
    ```
2.  **Get API Keys:**
    -   **Google Gemini:** Get `GOOGLE_API_KEY` from [Google AI Studio](https://aistudio.google.com/app/apikey).
    -   **Tavily:** Get `TAVILY_API_KEY` from [Tavily](https://tavily.com/).
3.  **Configure Keys:** Set `GOOGLE_API_KEY` and `TAVILY_API_KEY` as environment variables.
    -   *In Google Colab:* Use the Secrets panel (key icon).
    -   *Locally:* Use `export KEY='your-key'` (Linux/macOS) or `set KEY=your-key` (Windows).

## ▶️ How to Run

1.  Ensure setup is complete and API keys are accessible as environment variables.
2.  Run the Python script containing the agent code and workflow definition.
    -   *In Google Colab:* Open the notebook and run all cells sequentially.
    -   *Locally:* Save the code as a `.py` file and run `python your_script_name.py`.

The system will execute the multi-agent workflow and print the research steps and the final answer draft.

---
