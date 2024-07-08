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
Our investigation into LLMs' causal inference capabilities yielded mixed results. Previous studies, like Yang et al. (2023), found that most models only succeed at the first level of causal hierarchies. However, our experiments with UHHGPT models indicate that OpenAI's latest versions, particularly ChatGPT 4 Omni, perform better on benchmarks.  
ChatGPT 4 Omni outperformed its predecessor, ChatGPT 3.5 Turbo, and also Gemini recognizing complex relationships and subtle nuances more accurately. Despite this progress, issues with robustness remain. For example, minor input changes caused incorrect responses, questioning the model's reliability and true causal inference abilities.  
However, even though even ChatGPT 4 Omni will probably also have problems with some causal questions, it is hard to find these special cases. Also it is hard to distinguish between a better causal understanding in general, if ChatGPT 4.0 Omni can now answer questions that ChatGPT 3.5 Turbo used to answer incorrectly, or if this is just hardcoding of these special cases. (This is only known by OpenAI.) Issues like that definetly make it harder to test for causal inference capabilities of LLMs. 
These findings highlight the need for further research and robust evaluation methods to enhance LLMs. Future models should not only replicate existing causal information but also discover and accurately interpret new causal relationships. 

### References
[Linying Yang, Vik Shirvaikar, Oscar Clivio & Fabian Falck. 2023.](https://openreview.net/forum?id=mRwgczYZFJ)  
[Andrew K. Lampinen, Stephanie C. Y. Chan, Ishita Dasgupta, Andrew J. Nam & Jane X. Wang. 2023](https://doi.org/10.48550/arXiv.2305.16183)

