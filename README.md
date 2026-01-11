# ml-experiments
Experiments in Machine Learning and Deep Learning

## Prerequisites

- Python 3.11.9

## Environment Setup

### Installing Python 3.11.9

#### On Linux/Ubuntu:
```bash
# Using apt (if available)
sudo apt update
sudo apt install python3.11

# Or using pyenv (recommended for version management)
curl https://pyenv.run | bash
pyenv install 3.11.9
pyenv global 3.11.9
```

#### On macOS:
```bash
# Using Homebrew
brew install python@3.11

# Or using pyenv
brew install pyenv
pyenv install 3.11.9
pyenv global 3.11.9
```

#### On Windows:
1. Download Python 3.11.9 from [python.org](https://www.python.org/downloads/)
2. Run the installer and ensure "Add Python to PATH" is checked
3. Verify installation: `python --version`

### Setting Up the Project

1. Clone the repository:
```bash
git clone https://github.com/olgeorge/ml-experiments.git
cd ml-experiments
```

2. Create a virtual environment (recommended):
```bash
# Create virtual environment
python3.11 -m venv venv

# Activate virtual environment
# On Linux/macOS:
source venv/bin/activate

# On Windows:
venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

4. Verify the installation:
```bash
python -c "import numpy, pandas, sklearn, matplotlib; print('All libraries imported successfully!')"
```

## Getting Started

Launch the hello-world notebook to verify your setup:

```bash
jupyter notebook hello_world.ipynb
```

Or start Jupyter Lab:
```bash
jupyter lab
```

This notebook demonstrates:
- Basic NumPy operations
- Simple machine learning with scikit-learn
- Data visualization with matplotlib

## Project Structure

```
ml-experiments/
├── hello_world.ipynb    # Hello-world notebook with ML examples
├── requirements.txt     # Python dependencies
├── .gitignore          # Git ignore file
└── README.md           # This file
```

## Libraries Included

- **NumPy**: Numerical computing library
- **Pandas**: Data manipulation and analysis
- **scikit-learn**: Machine learning library
- **matplotlib**: Data visualization
- **Jupyter**: Interactive notebook environment

## Troubleshooting

### Virtual Environment Issues
If you encounter issues activating the virtual environment, ensure you're using the correct Python version:
```bash
python3.11 --version  # Should show Python 3.11.9
```

### Installation Errors
If package installation fails, try updating pip first:
```bash
pip install --upgrade pip setuptools wheel
```

### Jupyter Kernel Not Found
If Jupyter can't find the Python kernel:
```bash
python -m ipykernel install --user --name=venv
```
