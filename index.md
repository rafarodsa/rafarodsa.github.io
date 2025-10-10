---
layout: default
title: Rafael Rodriguez Sanchez
---

# About Me

<img class="profile-picture" src="profile.jpg">

I am a final year Ph.D. student in [Computer Science at Brown University](https://cs.brown.edu) in the [Intelligent Robot Lab](http://irl.cs.brown.edu) advised by [George Konidaris](http://cs.brown.edu/people/gdk/). Previously, I got a Bachelor's degree in Electronic Engineering from Universidad Simon Bolivar, Caracas, Venezuela and a Master's degree in Computer Science from [Politecnico di Milano](https://polimi.it) where I was fortunate to work with [Marcello Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml) and [Nicola Gatti](https://gatti.faculty.polimi.it) at the AIRLAB.
During Summer 2021, I interned at Amazon Alexa and worked in the Dialogue Research group with [Maryam Fazel-Zarandi](https://www.maryamfazel.com) using LLMs (Large Language Models) for semantic parsing via SFT (supervised finetuning) and RL in task-oriented dialog systems.


**Contact** rrs *at* brown *dot* edu --- **[Google Scholar](https://scholar.google.com/citations?user=ONxoqRUAAAAJ&hl=es)** --- **[LinkedIn](https://linkedin.com/in/rafarodsa)**
--- **[Github](https://github.com/rafarodsa)**

***Currently in the job market for Research Scientist positions***.

# Research Interests

<!-- I am deeply interested in enabling decision-making agents to learn reusable knowledge. To that end, currently, I'm working on learning state abstractions for Reinforcement Learning and, more generally, MDPs, that allow agents to learn provably sound, abstract and simpler world models that the agent can use to generate plans for different tasks.

Furthermore, I've also worked at the intersection of Natural Language and RL, investigating how to communicate prior knowledge to RL agents through languages. From this endeavor, RLang, a formal language for RL, was born. This language is unambiguous and designed precisely for RL. RLang allows to communicate partial task-specific knowledge to RL agents in order to avoid tabula rasa learning. The RLang framework, also, opens up many exciting research questions in RL algorithm design, natural language understanding and symbol grounding.  -->
<!-- 
During my Ph.D. my research has spanned representation learning [[factoredreps](#preprint-acf), [absreps](#conf-absmdp)], reinforcement learning and hierarchical RL [[vitransfer](#conf-transfer), [skillgraphs](#conf-skillgraphs)] . 
Specifically, I have focused on developing principled approaches to state representation learning that include abstraction [[absreps](#conf-absmdp)] and structure discovery [[factoredreps](#preprint-acf)] directly from high-dimensional observations. 
My research has leveraged advances in generative modeling, contrastive learning and energy-based modeling to implement practical algorithms to learn latent state representations. 

I've also worked at the intersection of Natural Language and RL [[rlang](#conf-rlang)], investigating how to communicate prior knowledge to RL agents through languages. From this endeavor, RLang, a formal language for RL, was born. This language is unambiguous and designed precisely for RL. RLang allows to communicate partial task-specific knowledge to RL agents in order to avoid tabula rasa learning. The RLang framework has inspired further research in natural language understanding and symbol grounding from an RL perspective [[nl2rlang](https://benjaminaspiegel.com/files/NL2RLang_RLC_2023_TAFM.pdf)].
While interning at Amazon Alexa, I gained hands-on experience in using LLMs for semantic parsing in task-oriented dialogs by finetuning via SFT and RL. -->

During my Ph.D., my research has focused on representation learning and reinforcement learning (RL), with an emphasis on developing principled approaches to state representation learning that include *abstraction* [[absreps](#conf-absmdp)] and *structure discovery* [[factoredreps](#preprint-acf)] directly from high-dimensional observations. I have leveraged advances in generative modeling, contrastive learning, and energy-based modeling to implement practical algorithms for learning latent state representations.

My work also explores the intersection of natural language and RL [[rlang](#conf-rlang)], investigating how to communicate prior knowledge to RL agents through language. This effort led to the development of RLang, a formal language for RL that allows the communication of partial, task-specific knowledge to agents—enabling them to learn more efficiently than in tabula rasa settings. The RLang framework has inspired further research in natural language understanding and symbol grounding from an RL perspective [[nl2rlang](https://benjaminaspiegel.com/files/NL2RLang_RLC_2023_TAFM.pdf)].

During my internship at Amazon Alexa, I gained hands-on experience applying large language models (LLMs) for semantic parsing in task-oriented dialogue systems, fine-tuning models via supervised learning (SFT) and reinforcement learning (RL).

<!-- # Publications

## **Preprints**
- **R. Rodriguez-Sanchez**, C. Allen, G. Konidaris. *From Pixels to Factors: Learning Independently Controllable State Variables for Reinforcement Learning*. Under review 2025.  
[<a href="#" onclick="toggleExpand('abstract_factor')">abstract</a>] [[paper](http://arxiv.org/abs/2510.02484)]
<div class="expandable-content" id="abstract_factor" style="display: none;">
Algorithms that exploit factored Markov decision processes are far more sample-efficient than factor-agnostic methods, yet they assume a factored representation is known a priori---a requirement that breaks down when the agent sees only high-dimensional observations. Conversely, deep reinforcement learning handles such inputs but cannot benefit from factored structure. We address this representation problem with Action-Controllable Factorization (ACF), a contrastive learning approach that uncovers independently controllable latent variables---state components each action can influence separately. ACF leverages sparsity: actions typically affect only a subset of variables, while the rest evolve under the environment's dynamics, yielding informative data for contrastive training. ACF recovers the ground truth controllable factors directly from pixel observations on three benchmarks with known factored structure---Taxi, FourRooms, and MiniGrid-DoorKey---consistently outperforming baseline disentanglement algorithms.
</div> 

## **Conferences**can

- A. Bagaria, A. De Mello Koch, **R. Rodriguez-Sanchez**, S. Lobel, G. Konidaris. *Intrinsically Motivated Discovery of Temporally
Abstract Graph-based Models of the World*. 2nd Reinforcement Learning Conference (RLC), Edmonton, Alberta, 2025.
[<a href="#" onclick="toggleExpand('abstract1')">abstract</a>] [[paper](https://openreview.net/pdf?id=vjT2aL6Wlg)]
<div class="expandable-content" id="abstract1" style="display: none;">
    We seek to design reinforcement learning agents that build plannable models of the world
    that are abstract in both state and time. We propose a new algorithm to construct a skill graph;
    nodes in the skill graph represent abstract states and edges represent skill policies. Previous
    works that learn a skill graph use random sampling from the state-space and nearest-neighbor
    search—operations that are infeasible in environments with high-dimensional observations (for
    example, images). Furthermore, previous algorithms attempt to increase the probability of all
    edges (by repeatedly executing the corresponding skills) so that the resulting graph is robust
    and reliable everywhere. However, exhaustive coverage is infeasible in large environments,
    and agents should prioritize practicing skills that are more likely to result in higher reward. We
    propose a method to build skill graphs that aids exploration, without assuming state-sampling,
    distance metrics, or demanding exhaustive coverage.
</div> 

- **R. Rodriguez-Sanchez**, G. Konidaris. *Learning Abstract World Models for Value-preserving Planning with Options*. 1st Reinforcement Learning Conference (RLC), Amherst, MA, 2024.  
[<a href="#" onclick="toggleExpand('abstract2')">abstract</a>] [[paper](https://openreview.net/pdf?id=h9IvopsMFS)] [[code](https://github.com/rafarodsa/abs-mdp)]
<div class="expandable-content" id="abstract2" style="display: none;">
    General-purpose agents require fine-grained controls and rich sensory inputs to perform a wide range of tasks. However, this complexity often leads to intractable decision-making. Traditionally, agents are provided with task-specific action  and observation spaces to mitigate this challenge, but this reduces autonomy. 
    Instead, agents must be capable of building state-action spaces at the correct abstraction level from their sensorimotor experiences. We leverage the structure of a given set of temporally-extended actions to learn abstract Markov decision processes (MDPs) that operate at a higher level of temporal and state granularity. We characterize state abstractions necessary to ensure that planning with these skills, by simulating trajectories in the abstract MDP, results in policies with bounded value loss in the original MDP.
    We evaluate our approach in goal-based navigation environments that require continuous abstract states to plan successfully and show that abstract model learning improves the sample efficiency of planning and learning.
</div> 

<img class="paper-picture" src="/rlang_logo.png">
- **R. Rodriguez-Sanchez**\*, B. Spiegel\*, J. Wang, R. Patel, S. Tellex, G. Konidaris. *RLang: A Declarative Language for Describing Partial World Knowledge to Reinforcement Learning Agents*. International Conference on Machine Learning (ICML). Honolulu, Hawaii, 2023. 
[<a href="#" onclick="toggleExpand('abstract3')">abstract</a>] [[paper](https://proceedings.mlr.press/v202/rodriguez-sanchez23a/rodriguez-sanchez23a.pdf)] [[RLang.ai](http://rlang.ai)] [[RLang package](https://github.com/brownirl/rlang)] 
<div class="expandable-content" id="abstract3" style="display: none;">
    We introduce RLang, a domain-specific language (DSL) for communicating domain knowledge to an RL agent. Unlike existing RL DSLs that ground to single elements of a decision-making formalism (e.g., the reward function or policy), RLang can specify information about every element of a Markov decision process. We define precise syntax and grounding semantics for RLang, and provide a parser that grounds RLang programs to an algorithm-agnostic partial world model and policy that can be exploited by an RL agent. We provide a series of example RLang programs demonstrating how different RL methods can exploit the resulting knowledge, encompassing model-free and model-based tabular algorithms, policy gradient and value-based methods, hierarchical approaches, and deep methods.
</div> 


- **R. Rodriguez-Sanchez**\*, [A. Tirinzoni](https://andreatirinzoni.github.io)\*, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transfer of Value Functions via Variational Methods*. Advances in Neural Information Processing Systems (NeurIPS), Montreal, Canada, 2018. 
[<a href="#" onclick="toggleExpand('abstract4')">abstract</a>] [[paper](https://proceedings.neurips.cc/paper_files/paper/2018/file/9023effe3c16b0477df9b93e26d57e2c-Paper.pdf)][[poster](/nips2018_poster_transfer.pdf)][[code](https://github.com/AndreaTirinzoni/variational-transfer-rl)]
<div class="expandable-content" id="abstract4" style="display: none;">
    We consider the problem of transferring value functions in reinforcement learning. We propose an approach that uses the given source tasks to learn a prior distribution over optimal value functions and provide an efficient variational approximation of the corresponding posterior in a new target task. We show our approach to be general, in the sense that it can be combined with complex parametric function approximators and distribution models, while providing two practical algorithms based on Gaussians and Gaussian mixtures. We theoretically analyze them by deriving a finite-sample analysis and provide a comprehensive empirical evaluation in four different domains.
</div>


## **Workshops**

- **R. Rodriguez-Sanchez**, C. Allen, G. Konidaris. *Disentangling Independently Controllable Factors in Reinforcement Learning*. The First New York Reinforcement Learning Workshop 2025. New York, NY.
[<a href="#" onclick="toggleExpand('abstract6')">abstract</a>][[extended abstract](/nyrl_2025__factored_reps.pdf)]

<div class="expandable-content" id="abstract6" style="display: none;">
    Leveraging the factored structure of the world leads to efficient algorithms for reinforcement learning that allows agents to abstract states, explore the world and discover skills. However, all these methods require access to a factored representation a priori. Typically, these representations are hand-specified and it remains an open problem how this representation can be learned directly from data. Therefore, applying these methods to problems with high-dimensional observations is not yet practical. In this work, we take a step toward factored representation in reinforcement learning. We introduce Action Controllable Factorization (ACF), a contrastive learning approach that focuses on disentangling *independently controllable* latent variables. These are variables the agent can affect directly without affecting others. The core idea of ACF is to leverage action sparsity: actions typically affect only a subset of variables, while the rest evolve under the environment's dynamics, yielding informative data for contrastive training. ACF recovers the ground‑truth controllable factors directly from pixel observations on three benchmarks with known factored structure---Taxi and MiniGrid‑DoorKey---consistently outperforming baseline disentanglement algorithms.
</div> 

- **R. Rodriguez-Sanchez**, G. Konidaris. *Learning Abstract World Models for Value-preserving Planning with Options*. Generalization in Planning at NeurIPS 2023 **(Contributed Talk)** and LatinX in AI Workshop. New Orleans, LA.  
[<a href="#" onclick="toggleExpand('abstract5')">abstract</a>][[Paper](/genplan2023.pdf)]

<div class="expandable-content" id="abstract5" style="display: none;">
    General-purpose agents require fine-grained controls and rich sensory inputs to perform a wide range of tasks. However, this complexity often leads to intractable decision-making. Traditionally, agents are provided with task-specific action  and observation spaces to mitigate this challenge, but this reduces autonomy. 
    Instead, agents must be capable of building state-action spaces at the correct abstraction level from their sensorimotor experiences. We leverage the structure of a given set of temporally-extended actions to learn abstract Markov decision processes (MDPs) that operate at a higher level of temporal and state granularity. We characterize state abstractions necessary to ensure that planning with these skills, by simulating trajectories in the abstract MDP, results in policies with bounded value loss in the original MDP.
    We evaluate our approach in goal-based navigation environments that require continuous abstract states to plan successfully and show that abstract model learning improves the sample efficiency of planning and learning.
</div>

<script>
function toggleExpand(elementId) {
    event.preventDefault();
    var content = document.getElementById(elementId);
    content.style.display = (content.style.display === "none") ? "block" : "none";
}
</script>

- **R. Rodriguez-Sanchez**, B. Spiegel, J. Wang, R. Patel, S. Tellex, G. Konidaris. *RLang: A Declarative Language for Expressing Prior Knowledge for Reinforcement Learning*. Multidisciplinary Conference on Reinforcement Learning and Decision Making (RLDM) 2022. Providence, RI.
[[paper](/rlang_rldm2022.pdf)] [[poster](/rlang_rldm_poster.pdf)]

- **R. Rodriguez-Sanchez**\*, [R. Patel](http://cs.brown.edu/people/rpatel59/)\*, [G. Konidaris](http://cs.brown.edu/people/gdk/). *On the Relationship Between Structure in Natural Language and Models of Sequential Decision Processes*. Language and Reinforcement Learning ([LaReL](https://larel-ws.github.io/accepted-papers/)) Workshop at the International Conference in Machine Learning (ICML) 2020. 
[[paper](/on_the_relationship_between_structure_in_natural_language_and_models_of_sequential_decision_processes.pdf)] [[video](https://www.youtube.com/watch?v=a3JJo_cvzpE&feature=emb_logo)]

- [A. Tirinzoni](https://andreatirinzoni.github.io), **R. Rodriguez-Sanchez**, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transferring Value Functions via Variational Methods*. European Workshop on Reinforcement Learning (EWRL) 2018. Lille, France. **Oral**. [[EWRL 2018](https://ewrl.wordpress.com/past-ewrl/ewrl14-2018/)]. -->


# For the community

- Single-ish file implementation of DreamerV3 in JAX [inspired by [Purejaxrl](https://github.com/luchris429/purejaxrl)]. 
[[repo](https://github.com/rafarodsa/dreamer-v3-purejax)].

# Publications

## **Preprints**
<a id="preprint-acf"></a>
[[factoredreps](#preprint-acf)] **R. Rodriguez-Sanchez**, C. Allen, G. Konidaris. *From Pixels to Factors: Learning Independently Controllable State Variables for Reinforcement Learning*. Under review 2025.  
[<a href="#" onclick="toggleExpand('abstract_factor')">abstract</a>] [[paper](http://arxiv.org/abs/2510.02484)]
<div class="expandable-content" id="abstract_factor" style="display: none;">
Algorithms that exploit factored Markov decision processes are far more sample-efficient than factor-agnostic methods, yet they assume a factored representation is known a priori---a requirement that breaks down when the agent sees only high-dimensional observations. Conversely, deep reinforcement learning handles such inputs but cannot benefit from factored structure. We address this representation problem with Action-Controllable Factorization (ACF), a contrastive learning approach that uncovers independently controllable latent variables---state components each action can influence separately. ACF leverages sparsity: actions typically affect only a subset of variables, while the rest evolve under the environment's dynamics, yielding informative data for contrastive training. ACF recovers the ground truth controllable factors directly from pixel observations on three benchmarks with known factored structure---Taxi, FourRooms, and MiniGrid-DoorKey---consistently outperforming baseline disentanglement algorithms.
</div> 

## **Conferences**
<a id="conf-skillgraphs"></a>
[[skillgraphs](#conf-skillgraphs)] A. Bagaria, A. De Mello Koch, **R. Rodriguez-Sanchez**, S. Lobel, G. Konidaris. *Intrinsically Motivated Discovery of Temporally
Abstract Graph-based Models of the World*. 2nd Reinforcement Learning Conference ***(RLC)***, Edmonton, Alberta, 2025.
[<a href="#" onclick="toggleExpand('abstract1')">abstract</a>] [[paper](https://openreview.net/pdf?id=vjT2aL6Wlg)]
<div class="expandable-content" id="abstract1" style="display: none;">
    We seek to design reinforcement learning agents that build plannable models of the world
    that are abstract in both state and time. We propose a new algorithm to construct a skill graph;
    nodes in the skill graph represent abstract states and edges represent skill policies. Previous
    works that learn a skill graph use random sampling from the state-space and nearest-neighbor
    search—operations that are infeasible in environments with high-dimensional observations (for
    example, images). Furthermore, previous algorithms attempt to increase the probability of all
    edges (by repeatedly executing the corresponding skills) so that the resulting graph is robust
    and reliable everywhere. However, exhaustive coverage is infeasible in large environments,
    and agents should prioritize practicing skills that are more likely to result in higher reward. We
    propose a method to build skill graphs that aids exploration, without assuming state-sampling,
    distance metrics, or demanding exhaustive coverage.
</div> 

<a id="conf-absmdp"></a>
[[absreps](#conf-absmdp)] **R. Rodriguez-Sanchez**, G. Konidaris. *Learning Abstract World Models for Value-preserving Planning with Options*. 1st Reinforcement Learning Conference ***(RLC)***, Amherst, MA, 2024.  
[<a href="#" onclick="toggleExpand('abstract2')">abstract</a>] [[paper](https://openreview.net/pdf?id=h9IvopsMFS)] [[code](https://github.com/rafarodsa/abs-mdp)]
<div class="expandable-content" id="abstract2" style="display: none;">
    General-purpose agents require fine-grained controls and rich sensory inputs to perform a wide range of tasks. However, this complexity often leads to intractable decision-making. Traditionally, agents are provided with task-specific action  and observation spaces to mitigate this challenge, but this reduces autonomy. 
    Instead, agents must be capable of building state-action spaces at the correct abstraction level from their sensorimotor experiences. We leverage the structure of a given set of temporally-extended actions to learn abstract Markov decision processes (MDPs) that operate at a higher level of temporal and state granularity. We characterize state abstractions necessary to ensure that planning with these skills, by simulating trajectories in the abstract MDP, results in policies with bounded value loss in the original MDP.
    We evaluate our approach in goal-based navigation environments that require continuous abstract states to plan successfully and show that abstract model learning improves the sample efficiency of planning and learning.
</div> 

<img class="paper-picture" src="/rlang_logo.png">
<a id="conf-rlang"></a>
[[rlang](#conf-rlang)] **R. Rodriguez-Sanchez**\*, B. Spiegel\*, J. Wang, R. Patel, S. Tellex, G. Konidaris. *RLang: A Declarative Language for Describing Partial World Knowledge to Reinforcement Learning Agents*. International Conference on Machine Learning ***(ICML)***. Honolulu, Hawaii, 2023. 
[<a href="#" onclick="toggleExpand('abstract3')">abstract</a>] [[paper](https://proceedings.mlr.press/v202/rodriguez-sanchez23a/rodriguez-sanchez23a.pdf)] [[RLang.ai](http://rlang.ai)] [[RLang package](https://github.com/brownirl/rlang)] 
<div class="expandable-content" id="abstract3" style="display: none;">
    We introduce RLang, a domain-specific language (DSL) for communicating domain knowledge to an RL agent. Unlike existing RL DSLs that ground to single elements of a decision-making formalism (e.g., the reward function or policy), RLang can specify information about every element of a Markov decision process. We define precise syntax and grounding semantics for RLang, and provide a parser that grounds RLang programs to an algorithm-agnostic partial world model and policy that can be exploited by an RL agent. We provide a series of example RLang programs demonstrating how different RL methods can exploit the resulting knowledge, encompassing model-free and model-based tabular algorithms, policy gradient and value-based methods, hierarchical approaches, and deep methods.
</div> 

<a id="conf-transfer"></a>
[[vitransfer](#conf-transfer)] **R. Rodriguez-Sanchez**\*, [A. Tirinzoni](https://andreatirinzoni.github.io)\*, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transfer of Value Functions via Variational Methods*. Advances in Neural Information Processing Systems ***(NeurIPS)***, Montreal, Canada, 2018. 
[<a href="#" onclick="toggleExpand('abstract4')">abstract</a>] [[paper](https://proceedings.neurips.cc/paper_files/paper/2018/file/9023effe3c16b0477df9b93e26d57e2c-Paper.pdf)][[poster](/nips2018_poster_transfer.pdf)][[code](https://github.com/AndreaTirinzoni/variational-transfer-rl)]
<div class="expandable-content" id="abstract4" style="display: none;">
    We consider the problem of transferring value functions in reinforcement learning. We propose an approach that uses the given source tasks to learn a prior distribution over optimal value functions and provide an efficient variational approximation of the corresponding posterior in a new target task. We show our approach to be general, in the sense that it can be combined with complex parametric function approximators and distribution models, while providing two practical algorithms based on Gaussians and Gaussian mixtures. We theoretically analyze them by deriving a finite-sample analysis and provide a comprehensive empirical evaluation in four different domains.
</div>


## **Workshops**
<a id="ws-nyrl"></a>
- **R. Rodriguez-Sanchez**, C. Allen, G. Konidaris. *Disentangling Independently Controllable Factors in Reinforcement Learning*. The First New York Reinforcement Learning Workshop 2025. New York, NY.
[<a href="#" onclick="toggleExpand('abstract6')">abstract</a>][[extended abstract](/nyrl_2025__factored_reps.pdf)]

<div class="expandable-content" id="abstract6" style="display: none;">
    Leveraging the factored structure of the world leads to efficient algorithms for reinforcement learning that allows agents to abstract states, explore the world and discover skills. However, all these methods require access to a factored representation a priori. Typically, these representations are hand-specified and it remains an open problem how this representation can be learned directly from data. Therefore, applying these methods to problems with high-dimensional observations is not yet practical. In this work, we take a step toward factored representation in reinforcement learning. We introduce Action Controllable Factorization (ACF), a contrastive learning approach that focuses on disentangling *independently controllable* latent variables. These are variables the agent can affect directly without affecting others. The core idea of ACF is to leverage action sparsity: actions typically affect only a subset of variables, while the rest evolve under the environment's dynamics, yielding informative data for contrastive training. ACF recovers the ground-truth controllable factors directly from pixel observations on three benchmarks with known factored structure---Taxi and MiniGrid-DoorKey---consistently outperforming baseline disentanglement algorithms.
</div> 

<a id="ws-genplan"></a>
- **R. Rodriguez-Sanchez**, G. Konidaris. *Learning Abstract World Models for Value-preserving Planning with Options*. Generalization in Planning at NeurIPS 2023 ***(Contributed Talk)*** and LatinX in AI Workshop. New Orleans, LA.  
[<a href="#" onclick="toggleExpand('abstract5')">abstract</a>][[Paper](/genplan2023.pdf)]

<div class="expandable-content" id="abstract5" style="display: none;">
    General-purpose agents require fine-grained controls and rich sensory inputs to perform a wide range of tasks. However, this complexity often leads to intractable decision-making. Traditionally, agents are provided with task-specific action  and observation spaces to mitigate this challenge, but this reduces autonomy. 
    Instead, agents must be capable of building state-action spaces at the correct abstraction level from their sensorimotor experiences. We leverage the structure of a given set of temporally-extended actions to learn abstract Markov decision processes (MDPs) that operate at a higher level of temporal and state granularity. We characterize state abstractions necessary to ensure that planning with these skills, by simulating trajectories in the abstract MDP, results in policies with bounded value loss in the original MDP.
    We evaluate our approach in goal-based navigation environments that require continuous abstract states to plan successfully and show that abstract model learning improves the sample efficiency of planning and learning.
</div>

<script>
function toggleExpand(elementId) {
    event.preventDefault();
    var content = document.getElementById(elementId);
    content.style.display = (content.style.display === "none") ? "block" : "none";
}
</script>

- **R. Rodriguez-Sanchez**, B. Spiegel, J. Wang, R. Patel, S. Tellex, G. Konidaris. *RLang: A Declarative Language for Expressing Prior Knowledge for Reinforcement Learning*. Multidisciplinary Conference on Reinforcement Learning and Decision Making (RLDM) 2022. Providence, RI.
[[paper](/rlang_rldm2022.pdf)] [[poster](/rlang_rldm_poster.pdf)]

- **R. Rodriguez-Sanchez**\*, [R. Patel](http://cs.brown.edu/people/rpatel59/)\*, [G. Konidaris](http://cs.brown.edu/people/gdk/). *On the Relationship Between Structure in Natural Language and Models of Sequential Decision Processes*. Language and Reinforcement Learning ([LaReL](https://larel-ws.github.io/accepted-papers/)) Workshop at the International Conference in Machine Learning (ICML) 2020. 
[[paper](/on_the_relationship_between_structure_in_natural_language_and_models_of_sequential_decision_processes.pdf)] [[video](https://www.youtube.com/watch?v=a3JJo_cvzpE&feature=emb_logo)]

- [A. Tirinzoni](https://andreatirinzoni.github.io), **R. Rodriguez-Sanchez**, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transferring Value Functions via Variational Methods*. European Workshop on Reinforcement Learning ***(EWRL) 2018***. Lille, France. ***Oral***. [[EWRL 2018](https://ewrl.wordpress.com/past-ewrl/ewrl14-2018/)].