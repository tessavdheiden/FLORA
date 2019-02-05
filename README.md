# FLORA

FLORA: Future prediction of obstacle locations in traffic scenes for collision avoidances.

For training use: python -m scripts.train
For evaluation use: python -m scripts.evaluate_model

## Improve code
- [ ] Remove in generator builder the devision by 2 for bottleneck dim
- [ ] Organize code: Seperate dataset from model, delete simple lstm, seperate code in scripts, sgan into more folders (better naming)
- [ ] Refactor train.py (too long)
- [ ] Commit attention model in pooling and physical pooling, maybe remove if statements

## Cluster computing
- [ ] Make kubernetis work

## Improve model performance
- [ ] Pool every
- [ ] Make graph network
- [ ] Learn collision checking of oracle
- [ ] Incorporate infrastructure elements with rules (traffic lights, roundabouts, zebra walks)

## Model 
SafeGAN synergizes generative adversarial networks (GAN) for generating multiple “real” trajectories with a reward network to generate plausible trajectories penalizing collisions. The reward network, Oracle, is environmentally aware to prune trajectories which result in collision.
![safeGAN](images/architecture.png)

