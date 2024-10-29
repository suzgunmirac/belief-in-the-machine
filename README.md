# Belief in the Machine: Investigating Epistemological Blind Spots of Language Models

[![arXiv](https://img.shields.io/badge/arXiv-2410.21195-b31b1b.svg)](https://arxiv.org/abs/2410.21195) [![Paper page](https://huggingface.co/datasets/huggingface/badges/resolve/main/paper-page-sm-dark.svg)](https://sites.google.com/view/msuzgun/research/belief-in-the-machine)

## Abstract

As language models (LMs) become integral to fields like healthcare, law, and journalism, their ability to differentiate between fact, belief, and knowledge is essential for reliable decision-making. Failure to grasp these distinctions can lead to significant consequences in areas such as medical diagnosis, legal judgments, and dissemination of fake news. Despite this, current literature has largely focused on more complex issues such as theory of mind, overlooking more fundamental epistemic challenges. This study systematically evaluates the epistemic reasoning capabilities of modern LMs, including GPT-4, Claude-3, and Llama-3, using a new dataset, **KaBLE**, consisting of 13,000 questions across 13 tasks. Our results reveal key limitations. 

* *First*, while LMs achieve 86% accuracy on factual scenarios, their performance drops significantly with false scenarios, particularly in belief-related tasks. 
* *Second*, LMs struggle with recognizing and affirming personal beliefs, especially when those beliefs contradict factual data, which raises concerns for applications in healthcare and counseling, where engaging with a person's beliefs is critical. 
* *Third*, we identify a salient bias in how LMs process first-person versus third-person beliefs, performing better on third-person tasks (80.7%) compared to first-person tasks (54.4%). 
* *Fourth*, LMs lack a robust understanding of the factive nature of knowledge, namely, that knowledge inherently requires truth. 
* *Fifth*, LMs rely on linguistic cues for fact-checking and sometimes bypass the deeper reasoning. 

These findings highlight significant concerns about current LMs' ability to reason about truth, belief, and knowledge while emphasizing the need for advancements in these areas before broad deployment in critical sectors.

![Cover-Figure](https://github.com/suzgunmirac/belief-in-the-machine/blob/main/figures/CoverFigure.png)

![KaBLE-Seed-Data](https://github.com/suzgunmirac/belief-in-the-machine/blob/main/figures/HintonExample.png)

## Knowledge and Belief Language Evaluation (KaBLE) Dataset

![KaBLE-Seed-Data](https://github.com/suzgunmirac/belief-in-the-machine/blob/main/figures/SeedSentences.png)

### Raw Input

Please refer to the `/kable-dataset` directory to get access to the raw input files.

- Out dataset is also available through Hugging Face Datasets at [https://huggingface.co/datasets/turingmachine/kable](https://huggingface.co/datasets/turingmachine/kable)

![KaBLE-Tasks](https://github.com/suzgunmirac/belief-in-the-machine/blob/main/figures/KableTasks.png)

### Model Outputs

All model outputs are stored in the `/outputs` directory.

![Model-Outputs-1](https://github.com/suzgunmirac/belief-in-the-machine/blob/main/figures/Examples-1.png)

### Running Experiments and Evaluation

To conduct your own experiments, please feel free to modify and use the `run_experiments.py` file. Before executing this code, however, please ensure that you have installed all the required packages (e.g., `pip install -r requirements.txt`) and have exported all relevant OpenAI API keys and credentials to your local environment (e.g., `export OPENAI_API_KEY="YOUR_API_KEY"`).

Here is an example command to run the experiments:

```python
[TBD]
```


## Citation

If your work makes use of our model, data, or results, please cite our paper as follows:

```bibtex
@article{suzgun2024beliefmachine,
      title={Belief in the Machine: Investigating Epistemological Blind Spots of Language Models}, 
      author={Mirac Suzgun and Tayfun Gur and Federico Bianchi and Daniel E. Ho and Thomas Icard and Dan Jurafsky and James Zou},
      year={2024},
      eprint={2410.21195},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2410.21195}, 
}
```

## Related Studies

- [LLMs' Reading Comprehension Is Affected by Parametric Knowledge and Struggles with Hypothetical Statements](https://arxiv.org/abs/2404.06283) (Bosmov et al., 2024)
- [Simple Linguistic Inferences of Large Language Models (LLMs): Blind Spots and Blinds](https://arxiv.org/abs/2305.14785) (Bosmov et al., 2023)
- [Conditional and Modal Reasoning in Large Language Models](https://arxiv.org/abs/2401.17169) (Holliday et al., 2024)
- [Clever Hans or Neural Theory of Mind? Stress Testing Social Reasoning in Large Language Models](https://arxiv.org/abs/2305.14763) (Shapira et al., 2023)
- [Large Language Models Fail on Trivial Alterations to Theory-of-Mind Tasks](https://arxiv.org/abs/2302.08399) (Ullman, 2023)
- [Reasoning or Reciting? Exploring the Capabilities and Limitations of Language Models Through Counterfactual Tasks](https://arxiv.org/abs/2307.02477) (Wu et al., 2023)
- [Neural Theory-of-Mind? On the Limits of Social Intelligence in Large LMs](https://arxiv.org/abs/2210.13312) (Sap et al., 2022)
- [Dissociating Language and Thought in Large Language Models](https://www.cell.com/trends/cognitive-sciences/fulltext/S1364-6613(24)00027-5) (Mahowald et al., 2024)
- [OpenToM: A Comprehensive Benchmark for Evaluating Theory-of-Mind Reasoning Capabilities of Large Language Models](https://arxiv.org/abs/2402.06044) (Xu et al., 2024)
- [How FaR Are Large Language Models From Agents with Theory-of-Mind?](https://arxiv.org/abs/2310.03051) (Zhou et al., 2023)
- [EPITOME: Experimental Protocol Inventory for Theory Of Mind Evaluation](https://openreview.net/forum?id=e5Yky8Fnvj#all) (Jones et al., 2023)
- [HI-TOM: A Benchmark for Evaluating Higher-Order Theory of Mind Reasoning in Large Language Models](https://arxiv.org/abs/2310.16755) (He et al., 2023)
- [Understanding Social Reasoning in Language Models with Language Models](https://proceedings.neurips.cc/paper_files/paper/2023/hash/2b9efb085d3829a2aadffab63ba206de-Abstract-Datasets_and_Benchmarks.html) (Gandhi et al., 2023)
- [ToMChallenges: A Principle-Guided Dataset and Diverse Evaluation Tasks for Exploring Theory of Mind](https://arxiv.org/abs/2305.15068) (Ma et al., 2023)
- [Revisiting the Evaluation of Theory of Mind through Question Answering](https://aclanthology.org/D19-1598/) (Le et al., 2019)
- [Do Large Language Models Know What Humans Know?](https://onlinelibrary.wiley.com/doi/full/10.1111/cogs.13309) (Trott et al., 2023)
- [Sparks of Artificial General Intelligence: Early experiments with GPT-4](https://arxiv.org/abs/2303.12712) (Bubeck et al., 2023)
- [Evaluating Large Language Models in Theory of Mind Tasks](https://arxiv.org/abs/2302.02083) (Kosinski, 2023)
- [How Not to Test GPT-3](https://cacm.acm.org/blogs/blog-cacm/270142-how-not-to-test-gpt-3/fulltext) (Marcus and Davis, 2023)
- [Towards A Holistic Landscape of Situated Theory of Mind in Large Language Models](https://arxiv.org/abs/2310.19619) (Ma et al., 2023)

## Acknowledgements

We thank William Held, Wesley H. Holliday, Adam T. Kalai, Jacopo Tagliabue, Merve Tekgürler, Suproteem Sarkar, Emily Shen, Kyle Swanson, Angelina Wang, and Mert Yüksekgönül for their helpful comments and suggestions. We also thank the members of the James Zou Lab and the participants at the IX. CSLI Workshop on Logic, Rationality, and Intelligent Interaction at Stanford University. 
