## Qiskit setup
https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit

```bash
python3 -m venv .venv
```

```bash
source .venv/bin/activate
```
```bash
pip install qiskit
```
```bash
pip install --upgrade pip
```
```bash
 pip install jupyter
```
The tutorial I am following is slightly outdate. Within my created notebook I am expect to run
```
from qiskit import *
from qiskit.tools.visualization import plot_histogram
%matplotlib inline
```
Output
```
---------------------------------------------------------------------------
ModuleNotFoundError                       Traceback (most recent call last)
Cell In[1], line 2
      1 from qiskit import *
----> 2 from qiskit.tools.visualization import plot_histogram
      3 get_ipython().run_line_magic('matplotlib', 'inline')

ModuleNotFoundError: No module named 'qiskit.tools'
```
qiskit.tools was removed in Qiskit 1.0 (released early 2024). 
The plot_histogram function has moved to a separate package called qiskit-visualization.

## The Fix
Step 1: Install the visualization package in my terminal
```
pip install 'qiskit[visualization]'
```
Step 2: Update your import in the notebook:

``` 
from qiskit import *
from qiskit.visualization import plot_histogram
%matplotlib inline
```
Now plot_histogram now lives directly in qiskit.visualization

```bash
pip install qiskit-aer
```