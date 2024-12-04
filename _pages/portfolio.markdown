---
title: Portfolio
permalink: /portfolio/
classes: wide
toc: true
---

<style>
p {
    font-size: 12px;
}
.container {
    display: flex;
    justify-content: space-around;
    align-items: flex-start; /* Ensures alignment at the top even if one is taller */
}

img {
    width: 100%;
    height: auto; /* Maintains aspect ratio */
}

figcaption {
    text-align: left; /* Aligns caption text to the left */
}
</style>

<br>
<br>

# Human Brain Data Science
2020-2024
<div class="container">
    <figure style="width: 350px; margin: 10px;">
        <img src="/assets/images/fMRI/fmri_image_1" alt='image 1' />
        <figcaption>The experimental paradigm. 20 pairs of associated stimuli were repeatedly presented on the screen (10 object – fruit associations; 10 object – animal associations).</figcaption>
    </figure>
    <figure style="width: 450px; margin: 10px;">
        <img src="/assets/images/fMRI/fmri_image_2.gif" alt='image 2' />
        <figcaption> Informative brain ROIs across the brain. </figcaption>
    </figure>
</div>

**Summary**:
We investigated the challenges of applying multivariate pattern classification (MVPC) to whole-brain fMRI data for decoding cognitive brain states. Using adversarial attacks, we analyzed classification boundaries and found consistent BOLD patterns across subjects, even when whole-brain classifiers performed poorly. Results suggest low decoding success reflects signal noise accumulation rather than inter-subject variability, highlighting the potential of MVPC for understanding cognitive states at the single-subject level. 

**Methods**:
Deep Learning (PyTorch), Numerical Simulation (NumPy), Adversarial Attacks, Classical Machine Learning, fMRI.

**Publication**: 
Athanasiadis et al., (In preparation). Decoding of non-perceptual properties in functional magnetic resonance imaging data.

<br>
<br>


# Rodent Brain Data Science
2019-2023
<figure style="width: 600px; margin: 10px;">
    <img src="/assets/images/rodents/rodents_image_1" alt='image 1' />
    <figcaption>Data set: Schematic of the decoding process. Time-binned population vectors were used as input to a linear neural network that is trained to predict
binary class labels (R: right; L: left) as an output. </figcaption>
</figure>

<figure style="width: 600px; margin: 5px;">
    <img src="/assets/images//rodents/rodents_image_2" alt='image 1' />
    <figcaption> (A) Relevant time bins corresponding to previous experience (B) Population statistics from relevant time bin. Significantly higher firing rates are observed in relevant versus nonrelevant time bins. See our <a href="https://doi.org/10.1002/hipo.23619">paper</a> for more details.</figcaption>
</figure>

**Summary**:
We explored hippocampal mechanisms supporting short-term memory using a classifier-based decoding approach. By analyzing the brain data of rodents recorded by microelectrodes, we were able to identify sparse, low-rate neural activity predictive of prior sensory-motor experiences, across working and non-working memory tasks, and dependent on sensory-motor context familiarity. We published our results in the peer-reviewed journal *Hippocampus*.

**Methods**: 
Statistics, Regression Analysis, Hypothesis Testing, Linear and Non-Linear Classifiers, Adversarial Attacks, Electrophysiology.

**Publication**: 
Athanasiadis et al., (2024). Low rate hippocampal delay period activity encodes behavioral experience. Hippocampus, 34(8), 422-437. <https://doi.org/10.1002/hipo.23619>

<br>
<br>


# Classification Most Informative Directions (MIDs)
2019-2022
<div class="container">
    <figure style="width: 400px; margin: 10px;">
        <img src="/assets/images/mids/mids_image_1.eps" alt='image 1' />
        <figcaption> Illustration of the MID identification process. A classifier is trained using a 2-fold cross validation scheme. Adversarial attack methods are employed to move data points close to the decision boundary. MIDs are then identified by clustering (DBSCAN) locally orthogonal vectors (gold). Results are grouped, sorted and evaluated over all cross validation iterations. </figcaption>
    </figure>
    <figure style="width: 400px; margin: 10px;">
        <img src="/assets/images/mids/mids_image_2.eps" alt='image 2' />
        <figcaption>Examples of identified MIDs for linear (A) and non-linear (B) binary classification tasks. </figcaption>
    </figure>
</div>

**Summary**: Classification algorithms are usually viewed as a black-box, with the most influential features with respect to categorical predictions made, not being readily available to us. Often to acquire this information probing the classifier across the whole of the feature space is required which is computationally ineffective for high-dimensional datasets. 

I developed a framework  that takes advantage of adversarial attacks in order to probe and visuallise decision boundaries in a computationally efficient manner. The framework is capable of identifying the most informative directions (MIDs) for linear and non-linear classifiers in terms of weight vectors orthogonal to the decision hyperplane. Furthermore, the MIDs can be used as a denoising mechanism when applied directly on the input data, in order to sort out the input patterns responsible for the formation of the decision hypreplane (RPs).  

**Methods**: Deep /Machine Learning (PyTorch), Computer Vision, Adversarial Attacks, Clustering, Data Processing, Data Augmentation

**Publication**: 
Athanasiadis et al., (2024). Low rate hippocampal delay period activity encodes behavioral experience. Hippocampus, 34(8), 422-437. <https://doi.org/10.1002/hipo.23619>

**GitHub repo**: <https://github.com/MarkosAthanasiadis/adversarial-decoder>

<br>
<br>



# Permutation Test
2019-2020
<figure style="width: 500px; margin: 10px; text-align: center;">
    <img src="/assets/images/perms/perm_image_1.png" alt='image 1' />
    <figcaption>P-value designation by comparing the
CCR of the real labels (pink line) against a Null distribution of randomly permuted labels (black curve).</figcaption>
</figure>

**Summary**: The Significance Testing Framework is a Python-based tool designed for permutation testing on datasets. It provides functionality to assess the statistical significance of machine learning models' performance by comparing against shuffled label baselines.

**Methods**: Deep Learning (PyTorch), Data Augmentation, Synthetic Data Generation, Data Processing.

**Publication**: 
Athanasiadis et al., (2024). Low rate hippocampal delay period activity encodes behavioral experience. Hippocampus, 34(8), 422-437. <https://doi.org/10.1002/hipo.23619>

**GitHub repo**: <https://github.com/MarkosAthanasiadis/permutation-test>
