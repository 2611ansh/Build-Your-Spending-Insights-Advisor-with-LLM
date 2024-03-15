# TransactBot

This project is a Flask web application that allows users to analyze their credit card transactions and get insights on their spending habits using a Large Language Model (LLM). The application uses IBM's LLAMA-2 model to interpret user inquiries and provide relevant information from a SQLite database containing transaction records.

## Features

- Analyze credit card transactions by submitting natural language inquiries
- Get insights on spending patterns, categories, and amounts
- Receive advice and strategies to manage expenses and reduce spending
- Visualize transaction data in a tabular format on the web interface

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/2611ansh/Spending-Insights-Advisor-with-LLM.git
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up the SQLite database:

   ```bash
   python db.py
   ```

   This will create the `history.db` file and populate it with sample transaction data from the `transactions.csv` file.

## Usage

1. Start the Flask application:

   ```bash
   python app.py
   ```

2. Open your web browser and navigate to `http://localhost:5000`.

3. Enter your inquiry regarding credit card transactions in the provided text box and submit.

4. The application will display the response from the LLM, including the result of the SQL query, an explanation of the thought process, and advice on expense management.

## Project Structure

- `app.py`: The main Flask application file, containing routes and LLM integration.
- `db.py`: Contains functions for creating and connecting to the SQLite database.
- `model.py`: Sets up the IBM LLAMA-2 model and configures the LLM.
- `transactions.csv`: A sample CSV file containing credit card transaction data.

## Dependencies

The project relies on several Python libraries, including:

- Flask: Web framework for building the application.
- LangChain: Library for building applications with Large Language Models (LLMs).
- ibm_watson_machine_learning: IBM's library for accessing LLAMA-2 and other foundation models.
- sqlite3: Python library for working with SQLite databases.

For a complete list of dependencies, please refer to the `requirements.txt` file.

## Contributing

Contributions are welcome! If you find any issues or want to add new features, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
