# SAMAS: Situation-Aware Multi-Agent Simulation System (ICASSP 2026)

This is the official implementation of  
**"EMPOWERING ECONOMIC SIMULATION THROUGH SITUATION-AWARE LLM-DRIVEN GENERATIVE SYSTEM"**  
(**Accepted at ICASSP 2026**)

**by [Zhimei Chen](mailto:zhimei.chen@swun.edu.cn) and [Mu Chen](mailto:mu.chen@alumni.uts.edu.au)**  
(1) School of Economics, Southwest Minzu University  
(2) ReLER, Australian Artificial Intelligence Institute, University of Technology Sydney

## Overview

Modern economic simulations often struggle to capture the rich dynamics of real-world social systems. Traditional top-down models rely on assumptions like agent homogeneity and rational expectations, while classic Agent-Based Modeling (ABM) falls short in generalizing beyond predefined rules or reward functions.

**SAMAS (Situation-Aware Multi-Agent System)** introduces a novel LLM-driven generative simulation framework that integrates **long-term macroeconomic awareness** and **short-term trajectory-based awareness** into individual agents. Each agent is instantiated as a human-like decision-maker, informed by:

- 📚 **Long-Term Awareness (LA)**: Commonsense macroeconomic knowledge embedded in LLMs (e.g., past financial crises).
- 📈 **Short-Term Awareness (SA)**: Personalized memory derived from each agent's recent interactions, modeled with risk sensitivity and forgetting.

The system captures **group-level dynamics** (e.g., consumption patterns by occupation) and supports **multi-agent, multi-step economic simulations**, demonstrating superior performance in both:

- **Volatility Realism (VR)**: How well simulated variables (e.g., CPI, GDP) mimic real-world volatility  
- **Turning-Point Hit Rate (HR)**: How accurately the system predicts economic peaks and troughs

<p align="center">
  <img src="fig/system_diagram.png" alt="SAMAS Framework Diagram" width="700"/>
</p>

## Features

- 🧠 **LLM-based Agent Cognition**: Use GPT, DeepSeek, Grok, or other LLMs for rich decision-making
- 🔄 **Situation-Aware Memory Module**: Combine macroeconomic signals + micro-agent trajectories
- 👥 **Group-Aware Behavior Modeling**: Capture emergent group decisions via clustering (e.g., blue-collar vs. business owner)
- 📊 **Multi-level Evaluation**: Quantitative benchmarks across daily/monthly/yearly economic cycles

## Simulation Results

| Method               | Volatility Realism (%) ↑ | HR-d ↑ | HR-m ↑ | HR-y ↑ | Token Usage (M) ↓ |
|----------------------|--------------------------|--------|--------|--------|-------------------|
| Rule-based (Simple) | 51.8                     | 26.8   | 41.5   | 46.0   | -                 |
| RL-based             | 71.2                     | 32.0   | 49.8   | 55.4   | -                 |
| LLM-based (Simple)   | 75.8                     | 35.6   | 54.7   | 60.1   | 141.3             |
| **SAMAS (Ours)**     | **81.5**                 | **42.5** | **64.8** | **70.9** | **167.9**         |

## Code

Coming soon...

## Citation

If you find our work helpful, please consider citing:

```bibtex
@inproceedings{chen2026samas,
  title={Empowering Economic Simulation through Situation-Aware LLM-Driven Generative System},
  author={Zhimei Chen and Mu Chen},
  booktitle={Proceedings of the IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  year={2026}
}
```

## Contact

For questions or collaborations, please contact:  
📧 Zhimei Chen: zhimei.chen@swun.edu.cn  
📧 Mu Chen: mu.chen@alumni.uts.edu.au
