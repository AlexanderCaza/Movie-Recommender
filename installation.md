# How to Install Jupyter Notebooks and Miniconda

## Step 1: Install Miniconda

### **Windows:**

1. Download the Miniconda installer for Windows from the Miniconda website: [https://docs.conda.io/projects/miniconda/en/latest/](https://docs.conda.io/en/latest/miniconda.html).

2. Double-click the downloaded `.exe` file to run the installer.

3. Follow the on-screen instructions to install Miniconda. Choose the "Just Me" option for installation scope and the default installation location.

4. After installation, open the "Anaconda Prompt" or "Miniconda3" command prompt from the Start menu.

### **macOS:**

1. Download the Miniconda installer for MacoS from the Miniconda website: [https://docs.conda.io/projects/miniconda/en/latest/](https://docs.conda.io/en/latest/miniconda.html). NOTE: Newer Macs with the M1 chip should download `Miniconda3 macOS Apple M1 64-bit pkg`, older intel based Macs should download `Miniconda3 macOS Intel x86 64-bit pkg` instead.

2. Double-click the downloaded `pkg` file to run the installer.

3. Follow the on-screen instructions to complete the installation. When prompted, press Enter to accept the license agreement and select the default installation location.

### **Linux(Ubuntu):**

1. Open a terminal window.

2. Install Miniconda for Linux using the package manager (e.g., apt on Ubuntu):

    ```bash
    sudo apt update
    sudo apt install miniconda
    ```

3. Follow the on-screen instructions to complete the installation. When prompted, press Enter to accept the license agreement and select the default installation location.

## Step 2: Create a Conda Environment

1. Open a terminal or command prompt.

2. Create a new Conda environment and install Jupyter Notebook by running the following command:

    ```bash
    conda create -n myenv python=3.9
    ```

3. Activate the newly created environment:

    ```bash
    conda activate myenv
    ```

## Step 3: Install Jupyter Notebook

1. While the Conda environment is active, install Jupyter Notebook using the following command:

    ```bash
    conda install -c anaconda jupyter
    ```

## Step 4: Customize and Launch Jupyter Notebook

1. Install pandas, progressbar, and numpy in your system.

    ```bash
    pip install pandas
    pip install progressbar
    pip install numpy
    ```

2. (Optional) Customize your jupyter notebook to dark mode by running the following commands in your terminal.

    ```bash
    pip install jupyterthemes
    jt -t grade3
    ```

    More details can be found [here](https://saturncloud.io/blog/jupyter-notebook-dark-mode-a-step-by-step-guide/).

3. In the same terminal where your Conda environment is active, run the following command to start Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

4. This will open a new browser window or tab displaying the Jupyter Notebook interface.

Now you have successfully installed Jupyter Notebooks and Miniconda on your computer and can begin using them within your Conda environment.
