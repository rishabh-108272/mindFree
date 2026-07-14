# Multi-Agent Creative Collaboration Tool

A multi-agent creative collaboration system built with LangGraph and Python, enabling AI agents to work together on creative tasks.

## Project Structure

```
mindFree/
├── agents/          # Individual agent implementations
├── graph/           # LangGraph workflow and graph definitions
├── tests/           # Test suite
├── venv/            # Python virtual environment (not in git)
├── .env             # Environment variables (not in git)
├── .env.example     # Template for environment variables
├── .gitignore       # Git ignore rules
├── requirements.txt # Python dependencies
└── README.md        # This file
```

## Setup Instructions

### 1. Clone and Navigate to Project

```bash
cd /Users/madhavthankasala/julyProject/mindFree
```

### 2. Create Virtual Environment

The virtual environment has already been created. To activate it:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

Dependencies are already installed. If you need to reinstall:

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Copy the example environment file and add your API keys:

```bash
cp .env.example .env
```

Edit `.env` and add your API keys:
- `ANTHROPIC_API_KEY`: Your Anthropic API key (required)
- `LANGCHAIN_API_KEY`: Your LangSmith API key (optional, for tracing)

### 5. Verify Installation

Check that all packages are installed correctly:

```bash
python -c "import langgraph, langchain, langchain_anthropic; print('All packages imported successfully!')"
```

## Dependencies

- **langgraph** (>=0.2.0): Framework for building multi-agent workflows
- **langchain** (>=0.3.0): LLM application framework
- **langchain-anthropic** (>=0.2.0): Anthropic integration for LangChain
- **python-dotenv** (>=1.0.0): Environment variable management
- **langchain-core** (>=0.3.0): Core LangChain functionality
- **langsmith** (>=0.1.0): Tracing and monitoring (optional)

## Next Steps

1. **Define Agent Types**: Create agent classes in the `agents/` directory
2. **Build Graph Structure**: Define the workflow graph in the `graph/` directory
3. **Implement State Management**: Set up state schemas for agent communication
4. **Add Tests**: Write unit and integration tests in the `tests/` directory
5. **Create Entry Point**: Build a main script to run the multi-agent system

## Development

### Running Tests

```bash
pytest tests/
```

### Deactivating Virtual Environment

```bash
deactivate
```

## License

[Add your license here]

## Contributing

[Add contribution guidelines here]