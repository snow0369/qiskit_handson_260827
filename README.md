# Qiskit Hands-On (2026-08-27)

Hands-on notebooks for the Qiskit workshop.

## Notebooks

| Notebook | Description |
|---|---|
| [`Introduction_to_Qiskit_Codealong_Client.ipynb`](Introduction_to_Qiskit_Codealong_Client.ipynb) | Introduction to Qiskit: building circuits, the Bell circuit, and running on real IBM Quantum hardware via Qiskit Runtime. |
| [`grovers_algorithm_tutorial.ipynb`](grovers_algorithm_tutorial.ipynb) | Grover's algorithm from first principles: the search problem, the oracle and diffuser, running on a simulator and real hardware, a logic-based Minesweeper oracle, and exercises. |

## Running on Google Colab

Each notebook can be opened directly in Colab without installing anything locally:

1. Go to the notebook on GitHub (links above, or from the file list at the top of this repo).
2. Click the **"Open in Colab"** badge at the top of the notebook (each notebook has one), or open [colab.research.google.com/github](https://colab.research.google.com/github) and paste in this repo's URL: `snow0369/qiskit_handson_260827`.
3. In the first code cell, run the package install cell (each notebook has one near the top) to install Qiskit and its dependencies into the Colab runtime. This only needs to run once per session.
4. Run the rest of the notebook top to bottom (**Runtime > Run all**, or cell by cell).

No local Python environment or IBM Quantum account is required to run circuits on the simulator. Cells that submit jobs to real IBM Quantum hardware will prompt for an IBM Quantum API token, see the notebook's own instructions right before that cell.

### Notes for Colab

- Colab resets its runtime (and any installed packages) each time you start a new session, re-run the install cell if you restart.
- Image links in the notebooks point at `raw.githubusercontent.com` URLs in this repo so that figures render correctly in Colab, not just on GitHub. If you fork this repo, update those links to point at your fork.
- The `grovers_algorithm_tutorial.ipynb` hardware-execution section uses a `job_id` variable: leave it as `None` to submit a new job (this consumes real IBM Quantum queue time/account usage), or set it to a previously printed job ID to fetch that job's results instead of resubmitting.

## Running locally

```bash
git clone https://github.com/snow0369/qiskit_handson_260827.git
cd qiskit_handson_260827
pip install qiskit qiskit-aer qiskit-ibm-runtime matplotlib jupyter
jupyter notebook
```
