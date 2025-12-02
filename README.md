# My First Sentinel Notebook

This is a simple guide to creating a Jupyter notebook for Azure Sentinel. It includes instructions on how to create a Python virtual environment, install dependencies, and create a Jupyter notebook as well as a sample notebook containing all the initial setup code to get you started.


### Create & activate a Python virtual environment

**1. Create the venv**


```bash
python3 -m venv sentinel-notebooks
```

(You can replace `venv` with any name.)

**2. Activate it**

- **macOS/Linux**
    

```bash
source sentinel-notebooks/bin/activate
```

- **Windows (PowerShell)**
    

```powershell
.\sentinel-notebooks\Scripts\Activate.ps1
```

**3. Deactivate**

```bash
deactivate
```

No sources are needed for this one (standard Python functionality).

### Installing Dependancies

Jupyter Notebooks

```bash
pip3 install notebooks
```

Msticpy

```bash
pip3 install msticpy\[azsentinel]
```

## Creating a Jupyter Kernel 

This step creates a Jupyter kernel that is bound to the virtual environment. This step is very important as it allows you to use the virtual environment as a kernel in Jupyter notebooks.

```bash
python3 -m ipykernel install --user --name sentinel-notebooks --display-name "Python (sentinel-notebooks)"
```
### Creating our First Notebook 

Use the command below to start the Jupyter notebook server. If your browser does not oppen automatically, navigate to http://localhost:8888 in your browser.

```bash
jupyter notebook
```

You may follow the steps below to create your first notebook, alternativelt you can copy the notebook in this repository to your current working directory (i.e., this is where you ran `jupyter notebook`).

![Create a new Notebook.png](https://github.com/dewardvide/My-First-Sentinel-Notebook/blob/c170de27f9c5e215ed34b29aba0cd0229433e395/screenshots/Create%20a%20new%20Notebook.png)

Rename and save the notebook 

![Rename your Notebook.png](https://github.com/dewardvide/My-First-Sentinel-Notebook/blob/c170de27f9c5e215ed34b29aba0cd0229433e395/screenshots/Rename%20your%20Notebook.png)

Before running the code, make sure you select the correct kernel in this case it will be the `Python (sentinel-notebooks)` kernel that we created in our previous steps. 

![Select the kernel you created.png](https://github.com/dewardvide/My-First-Sentinel-Notebook/blob/c170de27f9c5e215ed34b29aba0cd0229433e395/screenshots/Select%20the%20kernel%20you%20created.png)

