# project-snets

Assignments for the course *Complex networks: theory and applications*

:date: Date: Jul 2019

:school: Master in *Communications and Computer Networks Engineering* at *Politecnico di Torino*

:page_facing_up: Report: [`latex/complex_net_report_senacheribbe.pdf`](latex/complex_net_report_senacheribbe.pdf)

## Description

The project consists of 4 assignments covering the topic of Complex Networks.

#### Assignment 1: Centrality indices
Using a real graph as input, different centralities measures are computed and compared: degree, Katz and betweenness centrality.

#### Assignment 2: Epidemic processes over the graph
Different epidemic processes are simulated on a real graph using a Monte Carlo approach: SI model, bootstrap percolation, bootstrap percolation (stocastic).

#### Assignment 3: Erdős–Rényi model
The Erdős–Rényi model (G(n,p) model) is simulated and its properties are tested for different values of `n` and `p` (up to `n=100000`).

#### Assignment 4: Barabási–Albert model
The Barabási–Albert model is simulated and its properties are tested for `n=100000`.

More information are available in the final report [`latex/complex_net_report_senacheribbe.pdf`](latex/complex_net_report_senacheribbe.pdf).   
The code is written in Python 3 using numpy, scipy (sparse matrix operations) and numba (JIT compilation).

## Run the code

To run the code, you need Python 3, Jupyter Notebook and the Python packages listed in [`requirements.txt`](requirements.txt).

### Using virtual environment

Create a virtual environment, install the package dependencies and add a custom kernel to Jupyter:

```
$ python -m venv venv
$ source venv/bin/activate
(venv) $ pip install -r requirements.txt ipykernel
(venv) $ ipython kernel install --user --name=project-snets
(venv) $ deactivate
```
Now you can simply run:
```
$ jupyter-notebook
```
and browse the code in the `assignment*/` folders.

## License

The source code is licensed under the [GNU GPLv3](LICENSE). The content of the report is licensed under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)