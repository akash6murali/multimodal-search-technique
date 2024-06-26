# Multimodal Semantic Search Technique

This is a simple project inspired by OpenAI's CLIP model.

## What is multimodal search techenique?
- Multimodal search allows querying across different data types (text, images, audio, video) simultaneously. CLIP is a prominent multimodal AI model that matches images with text. It uses a vision encoder and a text encoder to map both into a shared embedding space. CLIP is trained on vast image-text pairs using contrastive learning, enabling it to perform various tasks like image classification and search without specific fine-tuning. [OpenAI's CLIP model](https://openai.com/index/clip/).

## Datset used?
- For this project Flickr30k Dataset will be used. It contains 31,783 images collected from Flickr, each paired with 5 human-written English captions. The captions describe the contents and actions in each image, providing diverse textual descriptions.
<img src="https://github.com/akash6murali/multimodal-search-technique/blob/main/assets/flick30k.png" weight="20%">

## tokenizer and pretrained model used to extract the caption embeddings?
- Using the snowflake-artic-embed-mmodel which is one of top performing model in Massive Text Embedding Benchmark (MTEB) Leaderboard.
- has the max embedding dimension of 768 and max tokens of 512, memory usage of 0.41gb with fp32 precision.

## pretrained model trained on Imagenet dataset used to extract the image features
- Using the mobilenetV2 pretrained model which is one of top performing model in Image feature extraction and classification.
- has a 3.4 million parameters and 14mb in size and an input dimension 224x224 pixel.

## Code and Results?
- Refer the **image-text-multimodal.ipynb** notebook for detail code and results. 
