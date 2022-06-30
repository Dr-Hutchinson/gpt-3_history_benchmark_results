# Replication Study: GPT-3's Performance on Historical Fields in the MMMLU Benchmarks (May 2022)
## By Daniel Hutchinson
In January 2021, researchers in the field of machine learning introduced a set of benchmarks for measuring the performance of Large Language Models (LLMs) in three historical fields.[^1]
This replication study reexamines GPT-3’s performance on these benchmarks following the implementation of the GPT-3 Instruct model in January 2022.[^2] The resulting data records significant gains on these benchmarks, approaching expert-level accuracy (80%) in two of the three historical fields. These results approach the performance of Deepmind’s Chinchilla, the LLM currently achieving the highest accuracy on these benchmarks. [^3]

| LLM        | A.P. U.S. History | A.P. European History   | A.P. World History
| ------------- |:-------------:| :-----:| :---:
| GPT-3 (January 2021)      | 52.9% | 53.9% | 56.1%
| GPT-3 Instruct (May 2022)      | 74.8%      |  60.9% | 75.5%
| Chinchilla (March 2022) | 83.3%      |    78.8% | 85.2%

## Replication Method:
Using the Python script [`benchmarks.py`](https://github.com/Dr-Hutchinson/gpt-3_history_benchmark_results/blob/main/benchmarks_results.py), the benchmark questions released by Hendrycks were retested using OpenAI’s API for GPT-3. GPT-3’s responses were then compared against the published answers contained in the Hendrycks  benchmark sets. The results of each of those benchmarks are contained in this collection. Users can rerun GPT-3’s performance on these benchmarks at [_Can AIs Accurately Interpret History? A Digital History Experiment_](https://dr-hutchinson-gpt-3-challenge-app-f0wvs8.streamlitapp.com/)

## Credits
Many thanks to Dan Hendrycks for sharing the discipline-specific results for the historical fields contained in the MMMLU Benchmarks. 


[^1]:Dan Hendrycks, et al, “Measuring Massive Multitask Language Understanding,” [_arXiv_:2009.03300v3](https://arxiv.org/pdf/2009.03300.pdf) (January 2021), 2, 11. 
[^2]:Long Ouyang, et al, “Training language models to follow instructions
with human feedback,” [_arXiv_:2203.02155v1](https://arxiv.org/pdf/2203.02155.pdf) (March 2022). 
[^3]:Jordan Hoffmann, et al, “Training Compute-Optimal Large Language Models,” [_arXiv_:2203.15556v1](https://arxiv.org/pdf/2203.15556.pdf) (March 2022), 31, table A6. 

