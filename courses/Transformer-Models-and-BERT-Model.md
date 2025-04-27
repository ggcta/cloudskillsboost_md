---
id: 538
name: 'Transformer Models and BERT Model'
datePublished: 2024-06-25
topics:
- Encoder-Decoder Architecture
- BERT
- NLP
type: Course
url: https://www.cloudskillsboost.google/course_templates/538
---

# [Transformer Models and BERT Model](https://www.cloudskillsboost.google/course_templates/538)

**Description:**

This course introduces you to the Transformer architecture and the Bidirectional Encoder Representations from Transformers (BERT) model. You learn about the main components of the Transformer architecture, such as the self-attention mechanism, and how it is used to build the BERT model. You also learn about the different tasks that BERT can be used for, such as text classification, question answering, and natural language inference.This course is estimated to take approximately 45 minutes to complete.

**Objectives:**

- Understand the main components of the Transformer architecture.
- Learn how a BERT model is built using Transformers.
- Use BERT to solve different natural language processing (NLP) tasks.

## Introduction

In this module you will learn about the main components of the Transformer architecture, such as the self-attention mechanism, and how it is used to build the BERT model. You also learn about the different tasks that BERT can be used for, such as text classification, question answering, and natural language inference.

### Video - [Transformer Models and BERT Model: Overview](https://www.cloudskillsboost.google/course_templates/538/video/489216)

- [YouTube: Transformer Models and BERT Model: Overview](https://www.youtube.com/watch?v=sUCiDU8GhMA)

Hi. I'm Sanjana Reddy, a machine learning engineer at Google's Advanced Solutions Lab. There's been a lot of excitement around generative AI and all the new advancements, including new vertex AI features that are coming up, such as Gen AI Studio, Model Garden, Gen AI API. Our objective in this short session is to give you a solid footing on some of the underlying concepts that make all the Gen AI magic possible. Today I'm going to talk about transformer models and the BERT model. Language modeling has evolved over the years. The recent breakthroughs in the past ten years include the usage of neural networks to represent text, such as Word2vec an N-grams in 2013. In 2014, the development of sequence to sequence models such as RNN's and LSTM’s helped improve the performance of ML models on NLP tasks such as translation and text classification. In 2015, the excitement came with attention mechanisms and the models built based on it, such as Transformers and the Bert model. In this presentation we'll focus on Transformers. Transformers is based on a 2017 paper named Attention As All You Need. Although all the models before Transformers were able to represent words as vectors, these vectors did not contain the context and the usage of words changes based on the context. For example, bank and river bank versus bank in bank robber might have the same vector representation before attention mechanisms came about. A transformer is an encoder decoder model that uses the attention mechanism. It can take advantage of pluralization and also process a large amount of data at the same time. because of its model architecture, attention mechanism helps improve the performance of machine translation applications. Transformer models were built using attention mechanisms at the core. A transformer model consists of encoder and decoder. The encoder encodes the input sequence and passes it to the decoder and the decoder decodes the representation for a relevant task. The encoding component is a stack of encoders of the same number. The research paper that introduced Transformers stack six encoders on top of each other. Six is not a magical number. It's just a hyperparameter. The encoders are all identical in structure, but with different weights. Each encoder can be broken down into two sub layers. The first layer is called self attention. The input of the encode are first flows through a self attention layer, which helps to encode or look at relevant parts of the words as it encodes a central word in the input sentence. And the second layer is called a feedforward layer. The output of the self attention layer is fed to the feedforward neural network. The exact same feedforward neural network is independently applied to each position. The decoder has both the self attention and the feedforward layer, but between them is the encoder decoder, attention layer that helps a decoder focus on relevant parts of the input sentence. After embedding the words in the input sequence, each of the embedding vector flows through the two layers of the encoder. The word at each position passes through a self attention process. Then it passes through a feedforward neural network, the exact same network with each vector flowing through it separately. Dependencies exist between these paths in this self attention layer. However, the feedforward layer does not have these dependencies and therefore various paths can be executed in parallel while they flow through the feedforward layer. In the self attention layer, the input embedding is broken up into query, key, and value vectors. These vectors are computed using weights that the transformer learns during the training process. All of these computations happen in parallel in the model, in the form of matrix computation. Once we have the query key and value vectors, the next step is to multiply each value vector by the soft max score in preparation to sum them up. The intention here is to keep intact the values of the words you want to focus on and leave out a irrelevant words by multiplying them by tiny numbers like 0.001, for example. Next, we have to sum up the weighted value vectors which produces the output of the self attention layer at this position. For the first word, you can send along the resulting vector to the feedforward neural network. To sum up this process of getting the final embeddings, these are the steps that we take. We start with the natural language sentence embed each word in the sentence. After that, we perform multi-headed attention eight times in this case and multiply this embedded word with the respective weighted matrices. We then calculate the attention using the resulting Q K.V. matrices. Finally, we can concatenate the matrices to produce the output matrix, which is the same dimension as the final matrix that this layer initially got. There's multiple variations of transformers out there now. Some use both the encoder and the decoder component from the original architecture. Some use only the encoder and some use only the decoder. A popular encoder only architecture is Bert. Bert is one of the trained transformer models. Bert stands for bidirectional encoder representations from transformers and was developed by Google in 2018. Since then, multiple variations of Bert have been built. Today, Bert Powers Google Search. You can see how different the results provided by Bert are for the same search query. Before and after, Bert was trained in two variations. One model contains Bert Base, which had 12 stock of Transformers with approximately 110 million parameters, and the other Bert Large with 24 layers of transformers with about 340 million parameters. The Bert model is powerful because it can handle long input context. It was trained on the entire Wikipedia corpus and books corpus. The Bert model was trained for 1 million steps. Bert is trained on different tasks, which means it has multi-task objective. This makes Bert very powerful because of the kind of tasks it was trained on. It works at both a sentence level and at a token level. These are the two different versions of Bert that were originally released. One is Bert Base, which had 12 layers, whereas Bert Large had 24 layers. And compared to the original transformer, which had six layers. The way that Bert works is that it was trained on two different tasks. Task one is called a masked language model, where the sentences are masked and the model is trained to predict the masked words. If you were to train Bert from scratch, you would have to mask a certain percentage of the words in your corpus. The recommended percentage for masking is 15%. The masking percentage achieves a balance between too little and too much masking. Too little masking makes the training process extremely expensive, and too much masking removes the context of the model requires. The second task is to predict the next sentence. For example, the model is given two sets of sentences. Bert aims to learn the relationships between sentences and predict the next sentence given the first one. For example, sentence A could be a man went to the store and sentence B is he bought a gallon of milk. Bert is responsible for classifying if sentence B is in next sentence after sentence A. This is a binary classification task. This helps Bert perform at a sentence level in order to train Bert. You need to feed three different kinds of embeddings to the model for the input sentence. You get three different embeddings token segment and position embeddings. The token embeddings is a representation of each token as an embedding in the input sentence. The words are transformed into vector representations of certain dimensions. Bert can solve NLP tasks that involve tex classification as well. An example is to classify whether two sentences say my dog is cute and he likes playing are semantically similar. The pairs of input texts are simply concatenated and fed into the model. How does Bert distinguish the input in a given pair? The answer is to use segment embeddings. There is a special token represented by SEP that separates the two different splits of the sentence. Another problem is to learn the order of the words in the sentence. As you know, Bert consists of a stack of transformers. Bert is designed to process input sequences up to a length of 512. The order of the input sequence is incorporated into the position embeddings. This allows Bert to learn a vector representation for each position. Bert can be used for different downstream tasks. Although Bert was trained on mass language modeling and single sentence classification, it can be used for popular NLP tasks like single sentence classification. Sentence Pair Classification. Question Answering and single sentence tagging tasks. Thank you for listening.

### Video - [Transformer Models and BERT Model: Lab Walkthrough](https://www.cloudskillsboost.google/course_templates/538/video/489217)

- [YouTube: Transformer Models and BERT Model: Lab Walkthrough](https://www.youtube.com/watch?v=6hhvQb8tSPs)

Hi. I'm Sanjana Reddy, a machine learning engineer at Google's Advanced Solutions Lab. Welcome to the lab walkthrough for Transformer models and BERT model. In this lab walkthrough, we'll be going through classification using a Pre-Trained Bert model. You'll find the setup instructions in our GitHub repository. Let's get started. In order to work on this notebook, you'll need to log into Google Cloud, go into Vertex AI and click on Workbench. Make sure that you have a notebook created once a notebook instance has been created. Click on Open Jupyter Lab. Once you've followed the instructions in our GitHub repository, navigate to classify text with Bert in this notebook, we're going to learn how to load a Pre-Trained Bert model from TensorFlow hub and build our own classification using the Pre-Trained Bert model, we learn how to train a Bert model by fine tuning it before you get started. Note that this notebook requires a CPU because the training does take quite a bit of time. When you open this notebook, there is a setup instruction in order to set up a bert kernel to install all the required libraries for this notebook. For this notebook, we're going to be using TensorFlow and TensorFlow hub TensorFlow text, which is required to pre process the input for the BERT model. You can see that I'm checking if a GPU is attached and I see that I have one GPU attached to this notebook. In this notebook we're going to train a sentiment analysis model to classify movie reviews as either being positive or negative based on the text of the review, we're going to be working with the IMDB data set that you can download from this URL. Once we have downloaded the data set, we can examine the data to see what's in it. We see that we have 25,000 files that belong to two classes, positive and negative, and we're going to be using 20,000 files for training and the remaining 5000 for testing. A sample of this dataset shows you the movie review over here and an associated label. So for the one over here, we see that the label that is associated is negative and the one below here it's positive. Once we've examined our dataset and we're happy with that, we're going to load a Pre-Trained BERT model from TensorFlow hub. TensorFlow hub offers multiple different variations of BERT models in all different sizes. We're going to use a small BERT for today's notebook. So this bird model has four different layers. It has 512 hidden units, and it has eight attention heads. For every BERT model that we load from TensorFlow hub, it is associated with a corresponding pre-processing model. You can find the corresponding pre-processing model on TensorFlow hub as well. We're going to examine the pre processing model. So we have we're going to load the pre processing model we see in the previous step and we pass a sample text over here. So we just passed. This is an amazing movie and we're going to examine the output. The pre processing model gives us multiple outputs. The first is the input word ID. The input word ID is the idea of the words in the tokenized sentence. The pre-processing model also provides us the masking for each word. Every sentence is converted into a fixed length input, and it masks words that are not valid. So once we have pre processed our input text, we can use the loaded bird model from TensorFlow hub in this particular cell block. It doesn't really make any sense because we've not trained the model. This is just a random list of numbers at this point. But once you pass the pre process text into this bird model, you get certain embeddings. So in order to define our classification model, we start with an input layer. The input layer takes the raw text as input passes it on to the processing layer for pre-processing that converted into token IDs, bird IDs and mask IDs. The pre processed words are then passed to the Pre-Trained model. There is an argument here called trainable. Trainable here determines if you want to fine tune the Pre-Trained model using the new data that you're training with or not. In our example, we are setting trainable to true, which means that we're going to update the initial weights of the Pre-Trained model. Your decision to set this to true or false depends on two things whether you want to update the weights and second, on the size of your dataset, if you have a relatively small data set, it is recommended to set this to false so that you're not introducing noise into the pre-trained weights. But if you have a large enough dataset, you can set this to true. Once we have our pre-trained model, we pass it through a dense layer to get probabilities for each of our classes. This is what the output from the model is going to look like. The output is going to be a probability of whether this particular sentence is true, is positive or negative. Since we're working with a binary classification problem, we're going to use binary cross entropy as our loss function and the metric to optimize for is going to be binary accuracy for initializing our training by defining the optimizer. In our case, we're using Adam, which is a popular choice for neural network models. Once we initialize the training, we can start training using model dot fit. We can pass the train dataset and the validation dataset and the number of epochs that we want to train for. Once the model has trained, let's evaluate the performance of the model. So in our case we see that the model achieved an accuracy of 85%, which is pretty decent considering we only trained it for five epochs. You can potentially thwart the accuracy and loss over time in order to visualize the model's performance. We see that the training loss is going down and we could work on our validation loss a little bit. But for the sake of demonstration, we've only trained it for five epochs. Once you're satisfied with the model that you've trained, you can save the model using model dot safe model dot save export. So TensorFlow model to a local path. So the export path in this line is going to be a part in your notebook instance. Once you've saved your model, you can load it to get predictions. So in this example we have this is such an amazing movie. This movie was great. The movie was okay-ish, the movie was terrible. And we get predictions for each of these sentences based on the model that we have trained. If you would like to take this further and deploy your model on Vertex AI to get online predictions, you could take the locally saved model and export it to Vertex AI. in order to do this, you need to check the signature of the model to see how you can pass predictions to the model. The signature of the model shows you what is the first layer that is taking input. So once we have the locally saved model, we are going to push the model to Vertex’s Model Registry using these commands. In order to put the model in Vertex’s Model Registry, you need to ensure that you have a Google Cloud storage bucket. And these lines over here, let you create a bucket. If it doesn't already exist, we're going to copy the locally saved model using GS Utils CP which takes a locally saved model from the export pack and puts it in the Google Cloud storage bucket. Once the model is in the Google Cloud Storage bucket, we're going to upload it to Vertex AI's model registry. We're using the Python SDK in this case. So we have a platform dot model dot upload, which takes the model from Google Cloud Storage Bucket and puts it in the model registry. Once the model has been uploaded, we're ready to deploy the model on Vertex and get online predictions. In order to do this, we can use the Python SDK again so we can use uploaded model to deploy, which is a function that is going to do two things. One, it's going to create an end point, and two, it's going to upload the model to this particular endpoint. So you can see here that it's creating the endpoint, providing you the endpoint location. And then once the endpoint has been created, the model is deployed to this endpoint. This step is going to take around 5 to 10 minutes. When you run through your notebook. So just don't worry if it takes too long, once the model has been deployed to the endpoint, you're ready to get predictions from this endpoint so you can create an instance object. So using the signature of the model, we know that the name of the first input layer is text. So we're going to pass our review text to this particular key. We create this instances object that is going to be passed to the endpoint dot predictive function. And the endpoint our predict function is going to take this instance and it's going to give us predictions. So we can see for our first instance, I love the movie and highly recommend it. We have a prediction of 0.99. For it was an okay movie in my opinion. We have 84% and for I hated the movie, we have 2%, which means it's a negative sentiment. So this is how you can create a classification model from a pre-trained BERT model and then deploy it on Vertex to get online predictions.

### Quiz - [Transformer Models and BERT Model: Quiz](https://www.cloudskillsboost.google/course_templates/538/quizzes/489218)

#### Quiz 1.

> [!important]
> **What is a transformer model?**
>
> - [ ] A natural language processing model that uses convolutions to learn relationships between different parts of a sequence.
> - [ ] A deep learning model that uses self-attention to learn relationships between different parts of a sequence.
> - [ ] A machine learning model that uses recurrent neural networks to learn relationships between different parts of a sequence.
> - [ ] A computer vision model that uses fully connected layers to learn relationships between different parts of an image.

#### Quiz 2.

> [!important]
> **What does fine-tuning a BERT model mean?**
>
> - [ ] Training the model on a specific task by using a large amount of unlabeled data
> - [ ] Training the hyper-parameters of the models on a specific task
> - [ ] Training the model on a specific task and not updating the pre-trained weights
> - [ ] Training the model and updating the pre-trained weights on a specific task by using labeled data

#### Quiz 3.

> [!important]
> **What is the attention mechanism?**
>
> - [ ] A way of determining the similarity between two sentences
> - [ ] A way of predicting the next word in a sentence
> - [ ] A way of identifying the topic of a sentence
> - [ ] A way of determining the importance of each word in a sentence for the translation of another sentence

#### Quiz 4.

> [!important]
> **What are the encoder and decoder components of a transformer model?**
>
> - [ ] The encoder ingests an input sequence and produces a sequence of tokens. The decoder takes in the tokens from the encoder and produces an output sequence.
> - [ ] The encoder ingests an input sequence and produces a sequence of hidden states. The decoder takes in the hidden states from the encoder and produces an output sequence.
> - [ ] The encoder ingests an input sequence and produces a single hidden state. The decoder takes in the hidden state from the encoder and produces an output sequence.
> - [ ] The encoder ingests an input sequence and produces a sequence of images. The decoder takes in the images from the encoder and produces an output sequence.

#### Quiz 5.

> [!important]
> **What are the three different embeddings that are generated from an input sentence in a Transformer model?**
>
> - [ ] Embedding, classification, and next sentence embeddings
> - [ ] Convolution, pooling, and recurrent embeddings
> - [ ] Token, segment, and position embeddings
> - [ ] Recurrent, feedforward, and attention embeddings

#### Quiz 6.

> [!important]
> **What is the name of the language modeling technique that is used in Bidirectional Encoder Representations from Transformers (BERT)?**
>
> - [ ] Recurrent Neural Network (RNN)
> - [ ] Long Short-Term Memory (LSTM)
> - [ ] Gated Recurrent Unit (GRU)
> - [ ] Transformer

#### Quiz 7.

> [!important]
> **What are the two sublayers of each encoder in a Transformer model?**
>
> - [ ] Embedding and classification
> - [ ] Convolution and pooling
> - [ ] Recurrent and feedforward
> - [ ] Self-attention and feedforward

#### Quiz 8.

> [!important]
> **BERT is a transformer model that was developed by Google in 2018. What is BERT used for?**
>
> - [ ] It is used to diagnose and treat diseases.
> - [ ] It is used to solve many natural language processing tasks, such as question answering, text classification, and natural language inference.
> - [ ] It is used to train other machine learning models, such as Recurrent Neural Networks (RNNs) and Long Short-Term Memory (LSTM) networks.
> - [ ] It is used to generate text, translate languages, and write different kinds of creative content.

#### Quiz 9.

> [!important]
> **What kind of transformer model is BERT?**
>
> - [ ] Recurrent Neural Network (RNN) encoder-decoder model
> - [ ] Encoder-decoder model
> - [ ] Decoder-only model
> - [ ] Encoder-only model

### Link - [Transformer Models and BERT Model: Lab Resources](https://www.cloudskillsboost.google/course_templates/538/documents/489219)

- [Transformer Models and BERT Model: Lab Resources](https://github.com/GoogleCloudPlatform/asl-ml-immersion/blob/master/notebooks/text_models/solutions/classify_text_with_bert.ipynb)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
