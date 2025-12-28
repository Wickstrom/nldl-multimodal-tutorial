# Northern Lights Deep Learning Tutorial on Multimodal Learning


This repository contains notebooks and example code for a hands-on multimodal learning tutorial. Further down is an overview and a description of the task in the tuorial. What follows is a detailed descripton oof how to follow the tutorial and upload your results to the leaderboard of the tutorial.

## Tutorial Steps

### Step 1: Open the Notebook in Google Colab
[![Open the notebook in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Wickstrom/nldl-multimodal-tutorial/blob/main/multi_modal_tutorial.ipynb)

---

### Step 2: Enable GPU support

<div style="text-align: center;">
  <p>Click on "Edit" in the top menu:</p>
  <img src="images/enable_gpu_1.png" width="300">
</div>
<div style="text-align: center;">
  <p>Select "Change runtime type":</p>
  <img src="images/enable_gpu_2.png" width="300">
</div>
<div style="text-align: center;">
  <p>Select a GPU under "Hardware accelerator":</p>
  <img src="images/enable_gpu_3.png" width="300">
</div>

---

### Step 3: Run code and fill in missing fusion part

<div style="text-align: center;">
  <p>Run code by clicking this symbol (remember to run all cells from the top down):</p>
  <img src="images/run_code_1.png" width="300">
</div>
<div style="text-align: center;">
  <p>Fill in the missing code for fusing data:</p>
  <img src="images/run_code_2.png" width="300">
</div>

---

### Step 4: Generate Predictions

<div style="text-align: center;">
  <p>Generate predictions:</p>
  <img src="images/generate_preds_1.png" width="30%">
</div>
<div style="text-align: center;">
  <p>Predictions are stored here:</p>
  <img src="images/generate_preds_2.png" width="30%">
</div>
<div style="text-align: center;">
  <p>Predictions appear here:</p>
  <img src="images/generate_preds_3.png" width="30%" alt="Predictions saved">
</div>
<div style="text-align: center;">
  <p>Download predictions and upload <a href="https://www.kaggle.com/t/0198c654889a49c2b36d772e3175e9a9" target="_blank">here.</a></p>
</div>

### Step 4: Submit predictions on Kaggle:

- fill

---

## Description of task

You are working as a machine learning engineer in an international post sorting company, and your boss
has tasked you with solving a challenging problem. Customers often provide handwritten digits that
must be automatically classified as image data for efficiency, but the camera you have available frequently
fails and introduces a great deal of noise into the data. You come up with an idea to incorporate a
fail-safe into your system. In addition to writing the digits down, the customers will now also repeat
the digits into a microphone, thus creating both an audio and an image version of their desired digits.
Unfortunately, your available microphone is not of the best quality, and also frequently introduces noise in
the audio recordings. Nevertheless, you believe that processing both modalities at the same time will lead to
satisfactory performance.

To test your idea, you collect 17560 pairs of images and audio of digits with a corresponding label for
training. In addition, you also collect an independent set of 5859 pairs of images and audio of digits with a corresponding label to test your system.

##

The figure below shows pairs of samples from the provided dataset. For each sample, noise is added such that one modality is more noisy than the other, or both are slightly noisy. This means that there is al limit to how well the model can perform using only one modality. However, if both modalities are processed simultaneously, there should always be a clean view that has the necessary information to make a prediction.

![Random samples from the dataset](images/random_samples.png)
