# Dynamics of Spontaneous Topic Changes in Next Token Prediction
## Original Paper

https://arxiv.org/abs/2501.06382

**Abstract**

Human cognition is punctuated by abrupt, spontaneous shifts between topics—driven by emotional, contextual, or associative cues—a phenomenon known as spontaneous thought in neuroscience. In contrast, self-attention-based models rely on structured patterns over their inputs to predict each next token, lacking spontaneity. Motivated by this distinction, we characterize *spontaneous topic changes* in self-attention architectures and reveal divergences from *spontaneous human thought*. First, we establish theoretical results under a simplified, single-layer self-attention model with suitable conditions by defining a topic as a set of Token Priority Graphs (TPGs). Specifically, we demonstrate that (1) the model maintains the priority order of tokens related to the input topic, (2) a spontaneous topic change can occur only if lower-priority tokens outnumber all higher-priority tokens of the input topic, and (3) unlike human cognition, the longer context length or the more ambiguous input topic does not increase the likelihood of spontaneous change. Second, we empirically validate that the effect of input length or topic ambiguity persists in modern, state-of-the-art LLMs, underscoring a fundamental disparity between human cognition and AI behavior in the context of spontaneous topic changes. To the best of our knowledge, no prior work has explored these questions with a focus so closely aligned to human thought.

## Structure
- ```1_Training_only.ipynb```

  Train the 3 self-attention models on data from Topic A, Topic B, and mixed-topic, respectively. Required
functions from the following docs:
  - data_utils_m.py
  - nxt_token_solver_m.py
  - base_nonlinear.py
  - utils.py
  - train_utils_m.py
  - visualizer.py
- ```2_Generate_test_data.ipynb```

  Generate the test data with varying T and varying L.
  
- ```3_Convergence_and_priority_similarity.ipynb```

  Show the convergence plot and the priority similarity in mixed-topic scenario.

- ```4_LLM_API_calls.ipynb```

  Empirically investigate behavior on four frontier models with increasing input length and topic ambiguity: GPT-4o, Llama-3.3, Claude-3.7, and DeepSeek-V3.  
  
