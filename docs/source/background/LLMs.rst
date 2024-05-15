Brief explanation of Large Language Models (LLMs)
=================================================

Ever since the Turing Test was proposed in the 1950s, humans have explored the mastering of language intelligence
by machine. Language is essentially a complex, intricate system of human expressions governed by grammatical rules. It poses a
significant challenge to develop capable artificial intelligence (AI) algorithms for comprehending and grasping a language. As a major
approach, language modeling has been widely studied for language understanding and generation in the past two decades, evolving
from statistical language models to neural language models. Recently, pre-trained language models (PLMs) have been proposed by pretraining Transformer models over large-scale corpora, showing strong capabilities in solving various natural language processing (NLP)
tasks. Since the researchers have found that model scaling can lead to an improved model capacity, they further investigate the scaling
effect by increasing the parameter scale to an even larger size. Interestingly, when the parameter scale exceeds a certain level, these
enlarged language models not only achieve a significant performance improvement, but also exhibit some special abilities (e.g., incontext learning) that are not present in small-scale language models (e.g., BERT). To discriminate the language models in different
parameter scales, the research community has coined the term large language models (LLM) for the PLMs of significant size (e.g.,
containing tens or hundreds of billions of parameters). Recently, the research on LLMs has been largely advanced by both academia
and industry, and a remarkable progress is the launch of ChatGPT (a powerful AI chatbot developed based on LLMs), which has
attracted widespread attention from society. The technical evolution of LLMs has been making an important impact on the entire AI
community, which would revolutionize the way how we develop and use AI algorithms


Large language models (LLM)
---------------------------

Researchers find that scaling PLM (e.g., scaling model size or data size) oftenleads to an improved model capacity on downstream tasks
(i.e., following the scaling law ). A number of studies have explored the performance limit by training an ever
larger PLM (e.g., the 175B-parameter GPT-3 and the 540Bparameter PaLM). Although scaling is mainly conducted
in model size (with similar architectures and pre-training tasks), these large-sized PLMs display different behaviors
from smaller PLMs (e.g., 330M-parameter BERT and 1.5Bparameter GPT-2) and show surprising abilities (called emergent abilities ) in solving a series of complex tasks. For
example, GPT-3 can solve few-shot tasks through in-context learning, whereas GPT-2 cannot do well. Thus, the research
community coins the term “large language models (LLM)” for these large-sized PLMs , which attract increasing
research attention . A remarkable application of LLMs is ChatGPT2 that adapts the LLMs from the GPT
series for dialogue, which presents an amazing conversation ability with humans. We can observe a sharp increase of the
arXiv papers that are related to LLMs after the release of ChatGPT .
As discussed before, language model is not a new technical concept specially for LLMs, but has evolved with the
advance of artificial intelligence over the decades. Early language models mainly aim to model and generate text data,
while latest language models (e.g., GPT-4) focus on complex task solving. From language modeling to task solving, it is an
important leap in scientific thinking, which is the key to understand the development of language models in the research history.
From the perspective of task solving, the four generations of language models have exhibited different levels of model capacities. 

.. image:: docs\image\trizz.png
   :alt: the evolution process of language models in terms of the task solving capacity
   :width: 600px

At first, statistical language models mainly assisted in some specific tasks (e.g., retrieval or speech tasks), in
which the predicted or estimated probabilities can enhance the performance of task-specific approaches. Subsequently,
neural language models focused on learning task-agnostic representations (e.g., features), aiming to reduce the efforts
for human feature engineering. Furthermore, pre-trained language models learned context-aware representations that
can be optimized according to downstream tasks. For the latest generation of language model, LLMs are enhanced by
exploring the scaling effect on model capacity, which can be considered as general-purpose task solvers. To summarize,
in the evolution process, the task scope that can be solved by language models have been greatly extended, and the task 
performance attained by language models have been significantly enhanced.


 

.. image:: docs\image\llm2.png
   :alt: A timeline of existing large language models (having a size larger than 10B) in recent years.
   :width: 600px

The timeline was established mainly according to the release date (e.g., the submission date to arXiv) of the technical paper for a model. 
If there was not a corresponding paper, we set the date of a model as the earliest time of its public release or announcement.
We mark the LLMs with publicly available model checkpoints in yellow color. Due to the space limit of the figure, we only
include the LLMs with publicly reported evaluation results.