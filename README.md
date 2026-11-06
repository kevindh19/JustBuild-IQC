# JustBuild · IQC 2026

## Build a quantum consulting firm

Your first client has heard the hype. Help them decide what to do about it.

For [Intermountain Quantum Competition 2026](https://intermountainquantum.org/), your team is a quantum computing consulting agency. Choose an imaginary company, a specific need, and a related quantum algorithm. Brief the JustBuild judges as your client: technical people with **no quantum computing background**.

**You are expected to deliver two things - a working Jupyter notebook and a slide deck.** Tell a cohesive story about what quantum computing can do, what your experiment demonstrates, and whether the company should invest.

## The challenge

1. **Choose your client.** What problem does their company address? Note - as you brainstorm who your (imaginary) client might be, remember that quantum algorithms are especially good for optimization problems.
2. **Create a cohesive story**. Figure out what the hype is behind quantum computing and why the company was interested in consulting. Prepare to explain the potential strengths and pitfalls of quantum computing - the judges have limited experience with quantum computing but are technically adept in AI engineering.
3. **Learn and run an algorithm.** Pick an algorithm that addresses the client's need. Create code to run the algorithm on a small problem and present the results of your algorithm (use **qBraid or Classiq**!). Simulators qualify for full credit; quantum hardware is optional. Teams are graded based on demonstrated understanding of the algorithm and results.
4. **Tie it all together.** Ultimately, you are to recommend the client either invest or pass on quantum computing. Provide enough data, both in explaining quantum computing and showing results/graphs, such that the client can make an informed decision.

## Tips
- It's better to have a simpler algorithm that you understand than a more efficient algorithm with mysterious AI generated code. Teams are encouraged to use AI models to learn, find resources, and code, with the expectation that they can explain what the algorithm does.
- Record how you use qBraid or Classiq as you generate and run code. Include this information on the Devpost submission.
- Reach out to mentors with expertise. The hacking area will have faculty members with experience in quantum information.
- We've generated some quantum algorithm tutorials in /notebooks to get you started; using AI to understand the concepts in each notebook, and how the code works, is highly recommended. The folder also contains three PDF tutorials.

## An example client

> “We manufacture wireless temperature sensors in Utah. We test each firmware release and coordinate when our sensors transmit. We've heard quantum computers can try every possibility at once. Could that help us? We have one engineer available for a week. How should we spend that time?”

You might try **Grover search** for a failing configuration or **QAOA** for grouping interfering sensors. Explain the gap between your toy model and a real firmware tester or radio network.

Other companies, problems, and algorithms are welcome. An evidence-based recommendation to **wait** is as valid as a recommendation to invest.

## What to submit

| Deliverable | What it should contain |
| --- | --- |
| **Executed Jupyter notebook** | Your problem, runnable quantum code, saved results and graphs, a classical comparison, and an interpretation. Record the platform, simulator or device, package versions, and rerun instructions. Credit sources and adapted examples. |
| **Slide deck** | Introduce the client and decision. Explain the relevant quantum basics, hardware versus software, and your algorithm. Present your experiment, address the hype and misconceptions, and end with a recommendation, risks, and a concrete next step. |

Connect the slides to the notebook's actual results. Distinguish what you demonstrated on a simulator from what would require future hardware or stronger evidence.

## How we'll judge

| Criterion | What we're looking for |
| --- | --- |
| **Working algorithm** | Runnable code, meaningful results, and a sensible classical check. |
| **Persuasive presentation** | A clear client story and a recommendation supported by evidence. |
| **Understanding of quantum computing** | Accessible explanations of the relevant ideas, capabilities, and limitations. |
| **Understanding of your algorithm** | You can explain its inputs, steps, outputs, assumptions, and connection to the client's need. |

## Start here

Follow the [setup guide](SETUP.md). These notebooks include diagrams, experiments, and briefing questions. **Start with 00, then choose one algorithm.**

| Walkthrough | What you'll learn |
| --- | --- |
| [00 · Quantum basics](notebooks/00_quantum_basics.ipynb) | Qubits, gates, interference, measurement, and reading a circuit. |
| [01 · Deutsch–Jozsa](notebooks/01_deutsch_jozsa.ipynb) | Learn a property of a function—and why the problem's promise matters. |
| [02 · Bernstein–Vazirani](notebooks/02_bernstein_vazirani.ipynb) | Recover a hidden bit pattern using interference. |
| [03 · Grover search](notebooks/03_grover_search.ipynb) | Amplify a desired result; see why more iterations can make it worse. |
| [04 · QAOA](notebooks/04_qaoa_maxcut.ipynb) | Combine a quantum circuit with classical optimization for a small graph problem. |

Deutsch–Jozsa and Bernstein–Vazirani are teaching problems with strong assumptions; a business analogy does not automatically make them useful business tools.

## Resources and ideas

- [Quantum Algorithm Zoo](https://quantumalgorithmzoo.org/): explore algorithms, problem types, and the assumptions behind claimed speedups.
- [IBM's quantum information course](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information): build the foundations behind your explanation.
- [qBraid Lab guide](https://docs.qbraid.com/v2/lab/user-guide/overview) and [Classiq's algorithm library](https://docs.classiq.io/explore/algorithms): find tools and examples to adapt.
