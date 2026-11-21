# AI Customer Support Quality Auditor

An AI-powered tool that automatically reviews customer support conversations and scores their quality, so teams can spot problems, coach agents, and improve customer satisfaction without manually reading every ticket.

## Features

- Analyzes support chats, emails, or call transcripts using an LLM
- Scores each conversation on criteria such as politeness, empathy, accuracy, clarity, and resolution
- Flags policy violations, rude or unprofessional language, and missed follow-ups
- Generates a short summary and improvement suggestions for each conversation
- Produces reports to track agent and team performance over time

## How It Works

1. **Input**: Load customer support conversations (text, CSV, or JSON).
2. **Audit**: Each conversation is sent to an AI model with a scoring rubric.
3. **Output**: The tool returns scores, flagged issues, and feedback.
4. **Report**: Results are saved or displayed for review.

## Getting Started

### Prerequisites

- Python 3.9 or higher
- An API key for your AI provider (for example OpenAI, Anthropic, or Gemini)

### Installation

```bash
git clone https://github.com/<your-username>/AI--Customer-Support-Quality-Auditor.git
cd AI--Customer-Support-Quality-Auditor
pip install -r requirements.txt
```

### Configuration

Create a `.env` file in the project root and add your API key:

```
API_KEY=your_api_key_here
```

Never commit this file. Make sure `.env` is listed in your `.gitignore`.

### Usage

```bash
python main.py
```

Replace `main.py` with your actual entry file (for example `app.py`) if it is named differently.

## Example Output

```
Conversation ID: 1042
Overall Score: 8.5 / 10
Politeness: 9   Empathy: 8   Accuracy: 9   Resolution: 8
Flags: None
Suggestion: Confirm with the customer that the issue is fully resolved before closing.
```

## Project Structure

```
AI--Customer-Support-Quality-Auditor/
├── main.py            # Entry point
├── requirements.txt   # Dependencies
├── data/              # Sample conversations
├── README.md
└── .env               # API keys (not committed)
```

Update this section to match your actual folders and files.

## Tech Stack

- Python
- Large language model API
- (Add any frameworks you use, such as Streamlit, Flask, or Pandas)

## Roadmap

- [ ] Dashboard for agent performance trends
- [ ] Support for multiple languages
- [ ] Custom scoring rubrics per team
- [ ] Export reports to PDF or CSV

## Contributing

Contributions are welcome. Fork the repo, create a branch, make your changes, and open a pull request.

## License

This project is licensed under the MIT License. Add a `LICENSE` file if you want to use this license.
