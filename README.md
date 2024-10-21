# Comparing GPT-2 Surprisal to Human N400 Responses to Novel Metaphors 

## Project Overview

This project aims to assess whether GPT-2 behaves similarly to humans, specifically in response to novel metaphors. 

How do pre-trained large language models (LLMs) interpret figurative language? Do these models process figurative language in an analogous way to humans, despite the absence of embodied experience? One prominent application of LLMs is to understand and model human language processing. Research in this area gives insight into how language statistics influences how we process language. Figurative language is particularly interesting because arriving at the true intended meaning requires that we are able to parse between literal and figurative interpretations. Whereas humans seem to do this implicitly, the question stands on whether LLMs share this ability, emergent solely from language statistics. [Tartter et al. (2002)](https://doi.org/10.1006/brln.2001.2610) addresses figurative language processing in humans, specifically in response to novel metaphors. The ERP recordings that were captured in this study show a robust N400 effect to anomalous sentence endings, but not for metaphorical or literal sentence endings.

In this analysis, I aim to explore whether GPT-2 responds similarly to novel metaphors as they do in the [Tartter et al. (2002)](https://doi.org/10.1006/brln.2001.2610) human ERP study. To achieve this, surprisal (the negative log probability) of the final word of each novel metaphor is calculated. Effects between conditions (`metaphor`, `anomaly`, and `literal`) are compared to the findings obtained from original human ERP study. 

## Python Packages Used

- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib.pyplot`, `seaborn` 
- **Others:** `torch`, `transformers`,`tqdm`

## Data

The stimuli used in this analysis is a subset of the stimuli used in the original [Tartter et al. (2002)](https://doi.org/10.1006/brln.2001.2610) study. It is located in the `data` folder of this repository.

## Results and Evaluation

The effects on surprisal obtained in this analysis seem to indicate that GPT-2 interprets novel metaphors as anomalous utterances. This is inconsistent with human ERP responses from the original study. Whereas the `metaphor` condition evoked lower N400 amplitudes than the `anomalous` condition in humans, the `metaphor` condition elicited the highest surprisal in GPT-2. 

These differences suggest that human language processing is fundamentally different from language processing performed by LLMs, such that humans may rely on other knowledge outside of language statistics—like embodied experience—to better parse between literal and figurative interpretations, ultimately arriving at the intended meaning much more efficiently. 

## License

[MIT License](https://opensource.org/license/mit/)

