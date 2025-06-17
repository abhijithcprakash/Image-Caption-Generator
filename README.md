---
# Image Caption Generator
Final project for the Building AI course

## Summary

This project is an AI-based system that takes an image as input and generates a relevant and meaningful caption for it. It combines computer vision and natural language processing to bridge the gap between images and text.

## Background

With the explosion of visual content on the internet, especially on platforms like Instagram, Facebook, and Pinterest, there's a growing need for automated tools that can describe images. Manually captioning thousands of images is time-consuming and expensive. This project aims to automate the task using AI.

Problems it addresses:

* Difficulty for visually impaired users to understand visual content
* Time-consuming manual image annotation for social media and dataset curation
* Content indexing and tagging for image search and recommendation engines

Personal motivation:
I am passionate about computer vision and its applications in accessibility and creative AI. Bridging visual understanding with language is one of the most fascinating challenges in AI today.

## How is it used?

The user uploads or provides an image to the system, and the model processes the image to generate a natural-language description. This can be used in:

* Accessibility tools (e.g., screen readers for visually impaired users)
* Social media content generation
* Automated dataset annotation
* Image search engine optimization

<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg" width="300">

Example output:
**Input Image:** A cat sleeping on its back
**Generated Caption:** "A sleepy cat lying on its back with paws in the air."

## Data sources and AI methods

Data source:

* [Flickr8k Dataset](https://forms.illinois.edu/sec/1713398) — a dataset of 8,000 images each with five captions
* [COCO Dataset](https://cocodataset.org/#home) — commonly used for image captioning tasks

AI Methods used:

* CNN (e.g., ResNet) for image feature extraction
* LSTM/Transformer for caption generation
* Encoder-Decoder architecture
* Tokenization and Beam Search/Greedy Decoding for better sentence formation

Example architecture:

```
Image → CNN → Feature Vector → LSTM Decoder → Caption
```

## Challenges

What it does not solve:

* It may not generate accurate captions for abstract or complex images.
* It doesn't recognize text embedded within images.
* The model may produce biased or inappropriate captions based on training data.

Ethical considerations:

* Ensuring the captions are fair and non-offensive
* Avoiding over-reliance on biased training datasets
* Clear disclosure when captions are AI-generated

## What next?

Future improvements:

* Use transformers (e.g., ViT + GPT) for better performance
* Multilingual caption generation
* Add speech output for visually impaired users
* Real-time deployment as a mobile or web application

To move forward, I’d need:

* Access to more diverse datasets
* Cloud GPU resources for training
* Collaboration with UI/UX designers for a frontend interface

## Acknowledgments

* [COCO Dataset by Microsoft](https://cocodataset.org/#home)
* [Flickr8k dataset by University of Illinois](https://forms.illinois.edu/sec/1713398)
* Inspiration from Andrej Karpathy's [NeuralTalk2](https://github.com/karpathy/neuraltalk2)
---
