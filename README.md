# Dynamics of Spontaneous Topic Changes in Next Token Prediction

## Documentation
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
  
