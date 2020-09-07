# audio-states-transitions
Accompanying code to paper [Investigating the Impact of Audio States & Transitions for Track Sequencing in Music Streaming Sessions](https://aaronng91.github.io/papers/recsys2020-audio-states.pdf) in RecSys '20.

## Requirements
- Python 3
- Tensorflow 2.0
- Tensorflow Probability 0.8
- matplotlib, pandas, scipy, numpy, seaborn

## Abstract
Music streaming is inherently sequential in nature, with track sequence information playing a key role in user satisfaction with recommended music. In this work, we investigate the role audio characteristics of music content play in understanding music streaming sessions. Focusing on 18 audio attributes (e.g. dancability, acousticness, energy), we formulate audio transitioning in a session as a multiple changepoint detection problem, and extract latent states of different audio attributes within each session. Based on insights from large scale music streaming data from a popular music streaming platform, we investigate questions around the extent to which audio characteristics fluctuate within streaming sessions, the heterogeneity across different audio attributes and their impact on user satisfaction. Furthermore, we demonstrate the promise of such audio-based characterizing of sessions in better sequencing tracks in a session, and highlight the potential gains in user satisfaction on offer. We discuss implications on the design of track sequencing models, and identify important prediction tasks to further research on the topic.

## Files
data_prep.ipynb - Code to prepare dataset used for experiments

full_analysis.ipynb - Code for analysis in Sections 3, 4.1, 4.2, 4.3

track_reranking_step1.ipynb and track_reranking_step2.ipynb - Code for track re-ranking experiment in Section 4.4

## Dataset
All experiments are done on a subset of Spotify's [Music Streaming Sessions Dataset](https://arxiv.org/abs/1901.09851), which can be obtained [here](https://www.aicrowd.com/challenges/spotify-sequential-skip-prediction-challenge).

## Reference
If you found the provided code useful, please consider citing our work.

Aaron Ng and Rishabh Mehrotra. **Investigating the Impact of Audio States & Transitions for Track Sequencing in Music Streaming Sessions.** In Fourteenth ACM Conference on Recommender Systems (RecSys ’20), September 2020.
