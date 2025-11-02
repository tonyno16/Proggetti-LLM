# AI Agent Instructions for LLM Projects

This repository contains various Language Learning Model (LLM) projects, with a focus on different AI model integrations and applications.

## Project Structure

```
.
├── Ollama/
│   └── Website-Summarizer/      # Web content summarization using Ollama
└── Open AI/                     # OpenAI-related projects
```

## Key Components

### Website Summarizer (Ollama Integration)

Located in `Ollama/Website-Summarizer/Ollama.ipynb`, this is a Jupyter notebook that demonstrates:

- Web scraping with BeautifulSoup
- Integration with Ollama's local API
- Markdown-formatted content generation
- Structured prompt engineering

Key architectural decisions:
- Uses `localhost:11434/api/chat` as the Ollama API endpoint
- Implements a `Website` class for content extraction and preprocessing
- Employs system and user prompts for consistent summarization

### Development Environment

Requirements:
- Python 3.13.5
- Jupyter Notebook environment
- Local Ollama installation running on port 11434
- Required Python packages:
  - requests
  - beautifulsoup4
  - ipython
  - ollama

## Working with the Code

### Website Summarizer Patterns

1. Content Extraction:
   ```python
   class Website:
       def __init__(self, url: str, timeout: int = 20):
           # Initialize with URL and timeout
           # Handles web scraping and content cleaning
   ```

2. Prompt Structure:
   - System prompt defines the AI assistant's role and output format
   - User prompt combines website title and cleaned content
   - All summaries are returned in Markdown format

### Testing

To test the website summarizer:
1. Ensure Ollama is running locally
2. Open `Ollama/Website-Summarizer/Ollama.ipynb`
3. Change the target URL in the last cell
4. Run all cells to generate a summary

## Best Practices

1. Content Preprocessing:
   - Remove navigation elements, scripts, and non-content HTML
   - Filter out lines with less than 2 words
   - Preserve meaningful text structure

2. Error Handling:
   - Implement timeouts for web requests
   - Handle missing website titles gracefully
   - Raise HTTP errors for failed requests

3. Output Formatting:
   - Use Markdown for structured summaries
   - Include bullet points for list items
   - Focus on main content, ignoring boilerplate

## Known Limitations

- Requires local Ollama installation
- Currently using gemma3:1b model
- Web scraping may need adjustments for complex sites