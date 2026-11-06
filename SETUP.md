# Run the walkthroughs

The five notebooks use **Qiskit in Python** and run independently. Begin with `00_quantum_basics.ipynb`, then pick one algorithm. You only need basic Python; the notebooks introduce the quantum concepts as you go.

All saved example outputs were generated **locally with an ideal simulator**, not on quantum hardware or a sponsor account. For your challenge submission, run your own experiment using **qBraid or Classiq** and record which platform and backend produced it.

## Option A · qBraid Lab

This is the direct route for the notebooks in this repository.

1. Sign in to [qBraid Lab](https://lab.qbraid.com/) and launch the Lab instance available to your event account. See the [getting started guide](https://docs.qbraid.com/v2/lab/user-guide/getting-started).
2. Download this repository from GitHub with **Code → Download ZIP**, unzip it, and upload the files to Lab, keeping the folder structure. Cloning the repository in Lab also works.
3. Use the [Environment Manager](https://docs.qbraid.com/v2/lab/user-guide/environments) to select a Qiskit environment and add its notebook kernel. The tested versions are in [requirements.txt](requirements.txt); you can use them when creating a custom Python 3.12 environment.
4. Open `notebooks/00_quantum_basics.ipynb` and select that kernel. If packages are missing or incompatible, run the following in a temporary notebook cell, then restart the kernel:

   ```python
   %pip install -r ../requirements.txt
   ```

5. Choose **Restart Kernel and Run All Cells**, read the diagrams, and try the prediction prompts. Save the notebook with its outputs before downloading or committing it.

The simulator is Qiskit's `Statevector`, running on the Lab computer. It calculates ideal amplitudes and samples measurement outcomes from them. It does not submit a remote QPU job or require an IBM API key. Exact state probabilities are a simulator teaching aid; physical hardware supplies measurement samples.

## Option B · Classiq

Use [Classiq's getting started guide](https://docs.classiq.io/getting-started) to access its platform and run a first model. The repository's Qiskit cells are **not Classiq SDK code**. You can learn from their experiments, then implement the same question with Classiq's Python SDK or Qmod.

- Start from an official [Deutsch–Jozsa example](https://docs.classiq.io/explore/algorithms/foundational/deutsch_jozsa/deutsch_jozsa), [Bernstein–Vazirani example](https://docs.classiq.io/explore/algorithms/foundational/bernstein_vazirani/bernstein_vazirani), or the [algorithm library](https://docs.classiq.io/explore/algorithms).
- To work in Jupyter, follow [Python SDK installation and authentication](https://docs.classiq.io/getting-started/sdk_installation). Keep the Classiq environment separate from these pinned Qiskit dependencies.
- Synthesize your model and run it on an available [Classiq simulator](https://docs.classiq.io/user-guide/execution/cloud-providers/classiq-backends). Record its name, parameters, shot count, and outputs.
- Submit a Jupyter notebook containing the runnable SDK workflow, plots, and explanation. If you develop in Qmod, include the model and the exact platform steps alongside your notebook's result analysis.

Classiq execution requires platform access. Keep authentication tokens out of your notebook and repository. Platform access and available compute depend on your event account; ask a sponsor mentor if setup is blocked.

## Local practice

Local practice is useful, but your submitted results should also have a documented qBraid or Classiq run. With Python 3.12, create a virtual environment from the repository root:

```bash
python -m venv .venv
```

Activate it with `.venv\Scripts\Activate.ps1` in Windows PowerShell, or `source .venv/bin/activate` on macOS/Linux. Then run:

```bash
python -m pip install -r requirements.txt
python -m jupyterlab
```

To check a notebook, choose **Restart Kernel and Run All Cells** in Jupyter. The dependencies were checked with Python 3.12.9; platform documentation links were reviewed on November 5, 2026.

## Before you submit

Restart and run the notebook from top to bottom. Replace the teaching example with your own experiment and client interpretation. Include the changed setting, your prediction, both results, a classical comparison, platform/backend details, and source credits. Save outputs so the judges can read your results without signing in to your account.
