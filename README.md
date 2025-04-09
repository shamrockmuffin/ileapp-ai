# iLEAPP AI

iLEAPP AI is a powerful iOS forensic analysis tool that leverages artificial intelligence to enhance digital forensic investigations. The tool provides comprehensive analysis capabilities for iOS device data, including message analysis, image analysis, and communication pattern detection.

## Features

- Message analysis and sentiment detection
- Image pattern recognition and analysis
- Communication chain analysis
- Comprehensive report generation
- Entity extraction and analysis
- Timeline generation

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ileapp-ai.git
cd ileapp-ai
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file with your OpenRouter API key:
```
OPENROUTER_API_KEY=your_api_key_here
```

## Usage

```python
from ileapp_ai.api.openrouter_client import OpenRouterClient
from ileapp_ai.analyzers.report_generator import ReportGenerator

# Initialize the client
client = OpenRouterClient()

# Generate a report
report_generator = ReportGenerator(client)
report = await report_generator.generate_report(analysis_data)
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
