---
id: 541
name: 'Introduction to Image Generation'
datePublished: 2025-04-10
topics:
- Image Processing
- Machine Learning Models
- Machine Learning
type: Course
url: https://www.cloudskillsboost.google/course_templates/541
---

# [Introduction to Image Generation](https://www.cloudskillsboost.google/course_templates/541)

**Description:**

This course introduces diffusion models, a family of machine learning models that recently showed promise in the image generation space. Diffusion models draw inspiration from physics, specifically thermodynamics. Within the last few years, diffusion models became popular in both research and industry. Diffusion models underpin many state-of-the-art image generation models and tools on Google Cloud. This course introduces you to the theory behind diffusion models and how to train and deploy them on Vertex AI.

**Objectives:**

- How diffusion models work
- Real use-cases for diffusion models
- Unconditioned diffusion models
- Advancements in diffusion models (text-to-image)

## Introduction to Image Generation

This course introduces diffusion models, a family of machine learning models that recently showed promise in the image generation space. Diffusion models underpin many state-of-the-art image generation models and tools on Google Cloud. This course introduces you to the theory behind diffusion models and how to train and deploy them on Vertex AI. 

### Video - [Introduction to Image Generation](https://www.cloudskillsboost.google/course_templates/541/video/530186)

- [YouTube: Introduction to Image Generation](https://www.youtube.com/watch?v=J0AuVBxzui0)

Hi. My name is Kyle Steckler, and I'm a machine learning engineer on the Advanced Solutions Lab team at Google Cloud. in this talk we're going to dive into an introduction to Image Generation. Specifically, I'll provide an introduction to diffusion models, a family of models that have recently shown tremendous promise in the image generation space. With that said, image generation has long been a field of interest, and there are many interesting approaches that you may have heard about. Now, while many approaches have been implemented for image generation, some of the more promising ones over time have been model families such as variational auto encoders, which encode images to a compressed size and then decode back to the original size while learning the distribution of the data itself. Generative adversarial models or Gans, have also been quite popular. These models are really interesting. They actually pit two neural networks against each other. One neural network, the generator creates images, and the other neural network, the discriminator predicts, if the image is real or fake. Over time, the discriminator gets better and better at distinguishing between real and fake, and the generator gets better and better at creating real looking fakes. You may have heard the term deepfakes before. And lastly, auto regressive models. These things generate images by treating an image as a sequence of pixels, and the modern approach with auto regressive models actually draws much of its inspiration from how LLM’s, or large language models, handle text. Very interesting. Now, in this talk, this is really going to be the focus and this is one of the newer image generation model families and that is diffusion models. Diffusion models draw their inspiration from physics, specifically thermodynamics. And while they were first really introduced for Image Generation in 2015, it took a few years for the idea to really take off. Within the last few years, though, 2020 up until now, we have seen a massive increase of diffusion models in both the research space and now today in the industry space as well. Diffusion models underpin many of the state of the art image generation systems that you may be familiar with today. Diffusion models show promise across a number of different use cases. Unconditioned diffusion models, where models have no additional input or instruction, can be trained from images of a specific thing, such as faces, as you can see on the slide here, and it will learn to generate new images of that thing. Another example of unconditioned generation is super resolution, which is really powerful at enhancing low quality images. We also have conditioned generation models and these give us things like text to image where we can generate an image from a text prompt and other things like image-inpainting and text guided image to image where we can remove or add things, we can edit the image itself. Now let's take a little bit of a deeper dove into diffusion models and talk about how do these things actually work. As noted on the slide here, the essential idea is to systematically and slowly destroy structure in a data distribution through an iterative forward diffusion process. Really, this is going to be adding noise iteratively to an image. We then learn a reverse diffusion process that restores structure in the data, yielding a highly flexible and tractable generative model of the data. In other words, we can add noise to an image iteratively, and we can then train a model that learns how to de-noise an image, thus generating novel images. So the goal here is that we want to have this model learn to de-noise, to remove noise. And in that aspect, then we could start here on the left of the slide. We could start from pure noise. And from that pure noise we could have a model that will be able to synthesize a novel image. Now, I know that there's a bit of math notation on this slide. So so let's break it down just a little bit. We start with a large dataset of images, but let's just take a single image here shown on the right hand side. Well, we can start this forward diffusion process and we can go from X zero. The initial image to X one, the initial image with a little bit of noise added to it. And we can do this over and over again. Iteratively adding more and more noise to the initial image. Now this distribution we call q and it only depends on the previous step. So if we do this over and over, iteratively adding more noise, we need to think about how many times do we perform that operation and the initial research paper did this 1000 times. So ideally, with that number being high enough, 1000 by the end of it, we should reach a state of pure noise. And so by this point, all structure in the initial image is completely gone. We're just looking at pure noise. Now, obviously, that's kind of the easy part. It's not too difficult to perform q, to iteratively add more and more noise. The challenging part is how do we go from a noisy image to a slightly less noisy image? And so this will refer to as the reverse diffusion process. And at this stage, every step of the way, every step that we add noise, we also learn the reverse diffusion process. That is, we train a machine learning model that takes in as input the noisy image and predicts the noise that's been added to it. Now let's look at that from a slightly different angle. We can visualize a single training step of the model here. So we have our initial image x on the left and we sample at a time step to create a noisy image. We then send that through our noisy model with the goal of predicting the noise. So the output of the model is the predicted noise, but we just added the noise to this image. We know what it is so we can actually compare that. We can see what is the difference between the model's predicted noise and the actual noise that we added. Now this model is trained similar to most machine learning models that you might be familiar with to minimize that difference. And over time, after seeing enough examples, this model gets very, very good at removing noise from images. And now for the fun part, this is where it gets really cool is we need to think about once we train this model, how do we generate images with it? Well, it's actually fairly intuitive. We can just start with pure, absolute noise and send that noise through our model that is trained. We then take the output, the predicted noise and subtract it from the initial noise. And if we do that over and over and over again, we end up with a generated image. Another way to think about this is that the model is able to learn the real data distribution of images that it's seen and then sample from that learn distribution to create new novel images. Very cool. As I'm sure we're all aware, there have been many advances in this space in just the last few years. And while many of the exciting new technologies on vertex AI for image generation are underpinned with diffusion models, lots of work has been done to generate images faster and with more control. Hopefully now, after taking a little bit of a look under the covers into how diffusion models work, you have a bit better intuition as to what's actually going on with these really new innovative model types. We've also seen wonderful results combining the power of diffusion models with the power of LLM’s, or large language models, that can really enable us to create context aware, photorealistic images from a text prompt. One great example of this is Imogen from Google Research. While it's a bit more complicated than what we've talked through in this session, you can see that at its core, it's a composition of an LLM and a few diffusion based models. This is a really exciting space and I'm thrilled to see this wonderful technology make its way into enterprise grade products on Vertex AI. Thanks for listening.

### Quiz - [Introduction to Image Generation: Quiz](https://www.cloudskillsboost.google/course_templates/541/quizzes/530187)

#### Quiz 1.

> [!important]
> **What are some challenges of diffusion models?**
>
> - [ ] All of the challenges listed are correct.
> - [ ] They can be difficult to control.
> - [ ] They can generate images that are not realistic.
> - [ ] They can be computationally expensive to train.

#### Quiz 2.

> [!important]
> **What is the name of the model family that draws inspiration from physics and thermodynamics?**
>
> - [ ] Diffusion models
> - [ ] Generative adversarial networks
> - [ ] Variational autoencoders
> - [ ] Autoregressive models

#### Quiz 3.

> [!important]
> **What is the process of forward diffusion?**
>
> - [ ] Start with a clean image and add noise randomly
> - [ ] Start with a noisy image and remove noise iteratively
> - [ ] Start with a noisy image and remove noise randomly
> - [ ] Start with a clean image and add noise iteratively

#### Quiz 4.

> [!important]
> **What is the goal of diffusion models?**
>
> - [ ] To pit two neural networks against each other
> - [ ] To learn the latent structure of a dataset by modeling the way in which data points diffuse through the latent space
> - [ ] To encode images to a compressed size, then decode back to the original size
> - [ ] To generate images by treating an image as a sequence of vectors

#### Quiz 5.

> [!important]
> **Which process involves a model learning to remove noise from images?**
>
> - [ ] Forward diffusion
> - [ ] GANs
> - [ ] Sampling
> - [ ] Reverse diffusion

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
