---
layout: default
title: Rafael Rodriguez Sanchez
---

# About Me

<img class="profile-picture" src="profile.jpg">

I am a fourth-year Ph.D. candidate in [Computer Science at Brown University](https://cs.brown.edu) in the [Intelligent Robot Lab](http://irl.cs.brown.edu) advised by [George Konidaris](http://cs.brown.edu/people/gdk/). Previously, I got a Bachelor's degree in Electronic Engineering from [Universidad Simon Bolivar](http://www.usb.ve), Caracas, Venezuela and a Master's degree in Computer Science from [Politecnico di Milano](https://polimi.it) where I was fortunate to work with [Marcello Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml) and [Nicola Gatti](https://gatti.faculty.polimi.it) at the [AIRLAB](http://airlab.deib.polimi.it). 

Moreover, in Summer 2021, I interned at Amazon Alexa and worked in the Dialogue Research group with Maryam Fazel-Zarandi on applications of LLMs (Large Language Models) and RL in Task-oriented Dialog Systems.


**Contact** rrs *at* brown *dot* edu --- **[Google Scholar](https://scholar.google.com/citations?user=ONxoqRUAAAAJ&hl=es)** --- **[LinkedIn](https://linkedin.com/in/rafarodsa)**
--- **[Github](https://github.com/rafarodsa)**

# Research Interests

I am deeply interested in enabling decision-making agents to learn reusable knowledge. To that end, currently, I'm working on learning state abstractions for Reinforcement Learning and, more generally, MDPs, that allow agents to learn provably sound, abstract and simpler world models that the agent can use to generate plans for different tasks.

Furthermore, I've also worked at the intersection of Natural Language and RL, investigating how to communicate prior knowledge to RL agents through languages. From this endeavor, RLang, a formal language for RL, was born. This language is unambiguous and designed precisely for RL. RLang allows to communicate partial task-specific knowledge to RL agents in order to avoid tabula rasa learning. The RLang framework, also, opens up many exciting research questions in RL algorithm design, natural language understanding and symbol grounding. 

# Publications

## ** Preprints**

- **R. Rodriguez-Sanchez**, G. Konidaris. *Learning Abstract World Models for Value-preserving Planning with Options*. Currently under submission. 

<a href="#" onclick="toggleExpand()">Abstract</a>

<div class="expandable-content" id="expandable-content" style="display: none;">
    General-purpose agents require fine-grained controls and rich sensory inputs to perform a wide range of tasks. However, this complexity often leads to intractable decision-making. Traditionally, agents are provided with task-specific action  and observation spaces to mitigate this challenge, but this reduces autonomy. 
    Instead, agents must be capable of building state-action spaces at the correct abstraction level from their sensorimotor experiences. We leverage the structure of a given set of temporally-extended actions to learn abstract Markov decision processes (MDPs) that operate at a higher level of temporal and state granularity. We characterize state abstractions necessary to ensure that planning with these skills, by simulating trajectories in the abstract MDP, results in policies with bounded value loss in the original MDP.
    We evaluate our approach in goal-based navigation environments that require continuous abstract states to plan successfully and show that abstract model learning improves the sample efficiency of planning and learning.
</div>

<script>
function toggleExpand() {
    var content = document.getElementById("expandable-content");
    content.style.display = (content.style.display === "none") ? "block" : "none";
}
</script>

## **Conferences**
<img class="paper-picture" src="/rlang_logo.png">
- **R. Rodriguez-Sanchez**, B. Spiegel, J. Wang, [R. Patel](http://cs.brown.edu/people/rpatel59/), S. Tellex, G. Konidaris. *RLang: A Declarative Language for Describing Partial World Knowledge to Reinforcement Learning Agents*. International Conference on Machine Learning (ICML). Hawaii, 2023. [[paper](https://arxiv.org/abs/2208.06448)] [[RLang.ai](http://rlang.ai)] [[RLang package](https://github.com/brownirl/rlang)] 

- [A. Tirinzoni](https://andreatirinzoni.github.io)\*, **R. Rodriguez-Sanchez**\*, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transfer of Value Functions via Variational Methods*. Advances in Neural Information Processing Systems (NeurIPS), Montreal, 2018. [[paper](/tirinzoni2018transfer.pdf)][[poster](/nips2018_poster_transfer.pdf)][[code](https://github.com/AndreaTirinzoni/variational-transfer-rl)]

## **Workshops**

- **R. Rodriguez-Sanchez**, B. Spiegel, J. Wang, R. Patel, S. Tellex, G. Konidaris. *RLang: A Declarative Language for Expressing Prior Knowledge for Reinforcement Learning*. Multidisciplinary Conference on Reinforcement Learning and Decision Making (RLDM) 2022. 
[[Paper](/rlang_rldm2022.pdf)] [[Poster](/rlang_rldm_poster.pdf)]

- **R. Rodriguez-Sanchez**\*, [R. Patel](http://cs.brown.edu/people/rpatel59/)\*, [G. Konidaris](http://cs.brown.edu/people/gdk/). *On the Relationship Between Structure in Natural Language and Models of Sequential Decision Processes*. Language and Reinforcement Learning ([LaReL](https://larel-ws.github.io/accepted-papers/)) Workshop at the International Conference in Machine Learning (ICML) 2020. 
[[paper](/on_the_relationship_between_structure_in_natural_language_and_models_of_sequential_decision_processes.pdf)] [[video](https://www.youtube.com/watch?v=a3JJo_cvzpE&feature=emb_logo)]

- [A. Bagaria](https://abagaria.github.io), [S. Kim](https://seungchan-kim.github.io), A. Mazzetto, **R. Rodriguez-Sanchez**. *Replication of a Unified Bellman Optimality Principle Combining Reward Maximization and Empowerment*. NeurIPS 2019 Replication Challenge. [[paper](https://openreview.net/pdf?id=B1grPT9GTH)]

- [A. Tirinzoni](https://andreatirinzoni.github.io), **R. Rodriguez-Sanchez**, [M. Restelli](https://restelli.faculty.polimi.it/MyWebSite/index.shtml). *Transferring Value Functions via Variational Methods*. European Workshop on Reinforcement Learning (EWRL) 2018. Lille, France. **Oral**. [[EWRL 2018](https://ewrl.wordpress.com/past-ewrl/ewrl14-2018/)].
