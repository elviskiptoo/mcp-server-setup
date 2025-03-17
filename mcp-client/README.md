# MCP Documentation Search Client

A tool for searching documentation across multiple Python libraries including LangChain, LlamaIndex, and OpenAI. This client uses the MCP server to provide fast and efficient documentation search capabilities.

## Features

- Asynchronous web scraping of documentation
- Supports searching across multiple library documentations
- Uses Google Search API through Serper for accurate results
- Easy integration with MCP server

## Prerequisites

- Python 3.7+
- A Serper API key (for Google Search functionality)
- MCP server installed

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd mcp-client
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install mcp-server python-dotenv beautifulsoup4 httpx
   ```

## Configuration

1. Create a `.env` file in the project root:
   ```env
   SERPER_API_KEY=your_serper_api_key_here
   ```

2. Get your Serper API key from [serper.dev](https://serper.dev) and add it to the `.env` file

## Usage

Run the client:


### Supported Libraries

You can search documentation for the following libraries:
- `langchain`: LangChain documentation (python.langchain.com/docs)
- `llama-index`: LlamaIndex documentation (docs/llamaindex.ai/en/stable)
- `openai`: OpenAI documentation (platform.openai.com/docs)

## API Reference

### get_docs(query: str, library: str)
Searches the documentation of the specified library for the given query.

Parameters:
- `query`: The search query (e.g., "How to use ChromaDB")
- `library`: The library to search in (one of: "langchain", "llama-index", "openai")

Returns:
- Text content from the documentation matching the query

## Contributing

1. Fork the repository
2. Create a new branch for your feature
3. Make your changes
4. Submit a pull request

## License

[Add your license information here]
