# Causal Reasoning of LLMs <a href="https://digitalcausalitylab.github.io/"><img src="figures/logo.png" align="right" width = "120" /></a>

This repository is created as a group project for the [Digital Causality Lab](https://digitalcausalitylab.github.io/).

### Participants

- Alexander Lorenz ([alexander.lorenz@studium.uni-hamburg.de](mailto:alexander.lorenz@studium.uni-hamburg.de))
- Jannik Svenson ([jannik.svenson@studium.uni-hamburg.de](mailto:jannik.svenson@studium.uni-hamburg.de))
- Lucas Mandelik ([lucas.mandelik@studium.uni-hamburg.de](mailto:lucas.mandelik@studium.uni-hamburg.de))

### Abstract
This project deals with the causal inference capabilities of Large Language Models (LLMs), using the article "A Critical Review of Causal Reasoning Benchmarks for Large Language Models" by Yang et al. (December 2023) as its foundation which examines various benchmarks to assess the ability of LLMs to perform causal inferences. Initially, we provide an overview of the articles main points, which include the introduction of two ability hierarchies.  
Firstly, the article introduces causal hierarchies, which represent different levels of causal statements that an LLM can correctly make based on situational and environmental information, discovering new knowledge from data, and predicting the quantitative impact of actions. Secondly, it describes the “ladder of causation,” which also has three levels: describing basic statistical associations, understanding the effect of interventions, and comprehending underlying causal mechanisms to make correct statements even for hypothetical scenarios. The complexity of tasks increases with each level for both hierarchies. According to the paper, most current models can handle the first level for both hierarchies but struggle with the second and third.  
Next, we conducted our own investigations by testing some of the questions proposed by the paper and other causal questions known to challenge LLMs. We used GPT 3.5 Turbo and GPT 4 Omni, both based on OpenAI's ChatGPT, and Gemini, provided by Google. Our investigation yielded mixed results. Previous studies indicated that most models only succeed at the first level of causal hierarchies. However, our experiments with the latest versions of OpenAI's models, particularly ChatGPT 4 Omni, show better performance on benchmarks. While ChatGPT 3.5 Turbo and Gemini show general weaknesses in causal reasoning, ChatGPT 4 Omni only displayed some robustness issues. These findings highlight that despite significant progress, LLMs are still far from achieving human-level causal reasoning capabilities.

### Current State and Call for Extension

- [Summary and Experimentation with popular current LLM Models] Briefly summarize the state of your data product as of the end of the course
- [Update findigs and test popular LLMs again or other + deeper research + maybe make a nice Tool representing Challenges for and Fails of LLMS] Briefly summarize what could be added or improved in the future

