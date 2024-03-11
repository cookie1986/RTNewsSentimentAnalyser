# RTNewsSentimentAnalyser
Performs real-time sentiment analysis of recent news articles based on user-specified keywords.

## Prerequisites

- Python 3.9
- Make


## Using the Makefile
The Makefile included simplifies the process of setting up the project environment and running the application. Below are the commands you can use:

### Setting Up the Virtual Environment
`make venv`: Creates a Python virtual environment and installs all required dependencies listed in requirements.txt. This command only needs to be run once at the beginning or whenever you update the dependencies in requirements.txt.

### Running the Application
`make run`: Activates the virtual environment and runs the main application script (main.py). Ensure you've set up the virtual environment using make venv before running this command.

### Cleaning Up
`make clean`: Removes Python bytecode files and the virtual environment directory. Use this command to clean up the project directory.

### Default Goal
If you run `make` without specifying a target, it will execute the `run` target by default, thanks to the .DEFAULT_GOAL setting in the Makefile.

### Notes
- The Makefile uses `.ONESHELL` special target which allows all commands in a recipe to run in a single shell instance. This is to enable activation of the virtual environment and execution of the subsequent commands within it.

- Ensure you have Python 3 and Make installed on your system to use these commands.
- This Makefile is designed to make it easier to manage project dependencies and streamline the execution of the code.