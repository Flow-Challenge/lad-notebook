# LAD-Notebook

## Description
It's a jupyter notebook to simplify the daily workflows of data developers by leveraging the power of Flow.

#Test comment

## Pre-Installation

### Mac

1. **Install Homebrew (if not already installed)**
   
   If you don’t have Homebrew installed, open Terminal and run:
   
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
   
   Once installed, verify it by running:
   
   ```
   brew --version
   ```

2. **Tap the Miniforge Repository**
   
   Miniforge is a lightweight Conda distribution available via Homebrew. Add the repository by running:
   
   ```
   brew tap homebrew/cask
   brew tap conda-forge/miniforge
   ```

3. **Install Miniforge**
   
   Install the lightweight Conda distribution (Miniforge) with:
   
   ```
   brew install --cask miniforge
   ```

4. **Initialize Conda**
   
   After installation, initialize Conda for your shell. Run:
   
   ```
   conda init
   ```

5. **Restart the Terminal**
   
   Close and reopen the Terminal to apply the changes.

6. **Verify Installation**
   
   Check if Conda is installed correctly by running:
   
   ```
   conda --version
   ```

7. **Update Conda (Optional)**

   Ensure you’re using the latest version:
   ```
   conda update -n base -c defaults conda
   ```


## Installation
To install and set up the project, follow the steps below:

1. Create a Conda environment:
   ```
   conda create --name lad-notebook python=3.11
   ```

2. Activate the Conda environment:
   ```
   conda activate lad-notebook 
   or
   source activate lad-notebook
   ```

3. Install the required packages:
   ```
   pip3 install -r requirements.txt
   ```

## Usage

To execute this project, you should use the `lad-notebook` conda. You have two options for running the Jupyter Notebook:

### Option 1: Run on Visual Studio Code
1. Open the project in Visual Studio Code.
2. Ensure you have the Jupyter extension installed. If not, you can install it from the Extensions Marketplace.
3. Select the lad-notebook kernel from the kernel picker in the top right corner of the notebook interface.
4. Start running your notebook directly in Visual Studio Code using `lad-notebook` as python kernel.

### Option 2: Start a Jupyter Server Locally
1. Ensure you have Jupyter installed in your environment. If not, install it using:
   ```bash
   pip install notebook
   ```

2. Start a Jupyter server using the following script:
   ```bash
   jupyter notebook
   ```
3. Open the notebook interface in your browser.
4. Select the lad-notebook kernel from the kernel menu.

#### Notes:
* Ensure the lad-notebook kernel is properly set up and linked to the environment required for this project.
* If you encounter issues selecting the kernel, check that the `ipykernel` package is installed in the environment:
   ```bash
   pip install ipykernel
   ```
* Let me know if you need help setting up the environment or troubleshooting!

## Contributing
Contributions are welcome! If you would like to contribute to this project, please follow the guidelines in the CONTRIBUTING.md file.

## License
This project is licensed under the [MIT License](LICENSE).
```