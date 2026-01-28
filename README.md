# ml-experiments
Experiments in Machine Learning and Deep Learning

## Environment Setup

Install Python 3.11.9

```bash
# Install pyenv via Homebrew
brew install pyenv

# Add pyenv to your shell configuration
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init --path)"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc

# Restart your shell or reload the configuration
source ~/.zshrc

# Install Python 3.11.9
pyenv install 3.11.9

# Set local version for this project (recommended)
cd ml-experiments
pyenv local 3.11.9
```

### Setting Up the Project

1. Clone the repository:
```bash
git clone https://github.com/olgeorge/ml-experiments.git
cd ml-experiments
```

2. Create a virtual environment (recommended):
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install --upgrade pip
pip install -r requirements.txt
```
