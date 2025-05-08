## Temporal and Uncertainty-aware Knowledge Graphs for Biomedical Literature


[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/baksho/ml-handson/blob/main/LICENSE)
[![Python 3.12.5](https://img.shields.io/badge/python-3.12.5-blue?logo=python&logoColor=ffffff)](https://www.python.org/downloads/release/python-3125/)
[![Pytorch 2.5.1](https://img.shields.io/badge/pytorch-2.5.1-orange?logo=pytorch&logoColor=ffffff)](https://pytorch.org/)
[![Keras 3.7.0](https://img.shields.io/badge/keras-3.7.0-red?logo=keras&logoColor=ffffff)](https://keras.io/)
[![TensorFlow 2.18.0](https://img.shields.io/badge/tensorflow-2.18.0-orange?logo=tensorflow&logoColor=ffffff)](https://www.tensorflow.org/)

#### Introduction

The biomedical research landscape is experiencing unprecedented growth, with over 1 million new papers published annually in PubMed alone. This massive influx of information creates significant challenges for researchers attempting to synthesize current knowledge. While recent advances in Natural Language Processing (NLP) and Knowledge Graph technologies have enabled automated extraction of biomedical relationships from literature, current systems fail to capture two critical dimensions: how scientific understanding evolves over time and the varying levels of certainty associated with extracted knowledge.

#### The Problem

Current biomedical knowledge systems suffer from several limitations:

1.	**Static representation**: Most knowledge graphs represent biomedical relationships as binary (exists/doesn't exist) rather than evolving entities that change as new evidence emerges.
2.	**Certainty blindness**: Extracted relationships are typically treated with equal confidence, failing to distinguish between well-established facts and emerging hypotheses.
3.	**Missing contradictions**: Systems rarely capture competing explanations or contradictory findings, leading to an incomplete picture of scientific discourse.
4.	**Temporal flattening**: The evolution of scientific understanding—including superseded theories, emerging consensus, and shifting paradigms—is lost in most knowledge representations.

As a result, researchers must manually track the historical development and confidence level of biomedical relationships, a process that becomes increasingly infeasible as literature volume grows.

#### Solution

We propose developing a *Temporal-Uncertainty Biomedical Knowledge Graph framework* that explicitly models both the evolution of scientific understanding and the confidence associated with biomedical relationships. Our system will:

1.	**Track temporal evolution**: Extract and represent when specific relationships were first proposed, gained acceptance, were challenged, or modified based on publication timestamps and citation patterns.
2.	**Model uncertainty levels**: Classify relationships on a spectrum from established facts to speculative hypotheses based on evidence patterns and consensus indicators.
3.	**Contradiction and Competing Theories**: How specific relationships have evolved over time, including competing explanations and periods of scientific controversy.

#### Technical Approach

Our implementation will combine:
- FAISS vector database to retrieve relevant papers based on the user query from the database
- Transformer-based NLP models fine-tuned for biomedical literature to extract relationships and their temporal context
- Temporal knowledge graph architectures with time-aware embeddings to represent varying certainty states
- Citation network analysis for tracking influence, consensus formation, and knowledge evolution



