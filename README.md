# LLM-Powered Metrics Query Processor 

A Python-based application that leverages the Groq LLM API to convert natural language queries about company performance metrics into structured JSON format. Perfect for analyzing company metrics and performing comparative analyses.

## Features

- **Natural Language Processing**: Convert human queries into structured data
- **Multi-company Comparison**: Compare metrics across different companies
- **Flexible Date Handling**: Support for both absolute and relative dates
- **Metric Normalization**: Handles various metric formats and abbreviations
- **Interactive Interface**: Real-time query processing
- **Conversation History**: Maintains context for follow-up queries

## Prerequisites

- Python 3.8+
- Groq API account and key
- VS Code with Jupyter extension (recommended)

## Initial Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/metrics-query-processor.git
cd metrics-query-processor
```

2. **Create and activate virtual environment**
```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# Unix/MacOS
python -m venv venv
source venv/bin/activate
```

3. **Install dependencies**
```bash
pip install groq python-dateutil 
```

4. **Configure API Key**
1. Visit [Groq Console](https://console.groq.com/)
2. Sign up/Login and navigate to API Keys section
3. Generate a new API key
4. Replace `your_groq_api_key_here` in Cell 1 with your actual API key

## Running the Application

### Step 1: Run All Cells in Order
Run each cell in sequence:
1. Cell 1: Imports and Setup
2. Cell 2: Date Handling Functions
3. Cell 3: Prompt Template
4. Cell 4: Main Processing Function
5. Cell 5: JSON Conversion Function
6. Cell 6: Main Application Class
7. Cell 7: Testing Functions
8. Cell 8: Example Usage and Testing
9. Cell 9: Interactive Query Interface

### Step 2: Start Interactive Interface
After running all cells, the interactive interface will start automatically. You'll see:
```
Welcome to the Metrics Query Processor!
==================================================

Example queries:
1. Get me Flipkart's GMV for the last one year
2. Compare Amazon and Walmart's revenue from last quarter
3. Show me Meta's profit between January 2023 and March 2024

Type 'exit' to quit, 'clear' to clear conversation history
==================================================
```

### Step 3: Using the Interactive Interface

#### Available Commands:
- Type your query and press Enter to process it
- Type 'exit' to quit the application
- Type 'clear' to reset conversation history

#### Example Interaction:
```
Enter your query:
> Get me Flipkart's GMV for last quarter

Processing query...

Result:
[
  {
    "entity": "Flipkart",
    "parameter": "GMV",
    "startDate": "2024-02-02",
    "endDate": "2024-05-02"
  }
]
```

## 3. Important Notes
- Ensure all cells are executed in order
- Wait for each cell to complete before running the next
- Make sure your Groq API key is valid
- Maintain active internet connection
- The interface will remember conversation context for up to 6 messages
- Use 'clear' command if you want to start a fresh conversation

## 4. Troubleshooting
If you encounter issues:
1. Check if all cells were executed in order
2. Verify your API key is correctly set
3. Ensure all dependencies are installed
4. Try clearing the conversation history
5. Restart the kernel and run all cells again if needed

## 5. Query Guidelines
For best results:
- Include company name and metric in your query
- Use supported date formats or relative dates
- Keep queries clear and specific
- Use comparison terms like "Compare with" or "Compare to" for multiple companies


## 📚 Notebook Structure

1. Imports and Setup
2. Date Handling Functions
3. Prompt Template
4. Main Processing Function
5. JSON Conversion Function
6. Main Application Class
7. Example Usage
8. Interactive Interface

## ⚠️ Error Handling

The application handles various error scenarios:
- Invalid API key
- Malformed queries
- Invalid date formats
- Network issues
- JSON parsing errors




