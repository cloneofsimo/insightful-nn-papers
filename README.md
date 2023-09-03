# Insightful Neural Network Papers

**Great job!**. You've finished your linear algebra, calculous, maybe good amount of probability theory, statistics and maybe even some course on optimization. You've gone through your assignments, written some code (perhaps with pytorch), and done some projects.

Now what? Before you jump into the hype-train like LLAMAs and Stable Diffusion, NeRFS etc etc, you should be aware: **the field is changing rapidly**. I've curated some of the *unique & foundational papers that you should read to understand the field better*. And by foundational, I mean insightful papers that explores stuff that are generally applicable to many different real-life problems. Deep learning and neural networks are exciting and have far more interesting literature other than just theory (I do think theory is *incredibly important* though).

You might even consider this as *survey of surveys* in neural network, as many of the literature I will mention here are extremely unique.

[WIP. I WILL ADD THEM AS I FIND MORE TIME]

## Generalization

[We need to rethink generalization]()

[Tendency to find low-rank solution]()

[Tendency to find smoother solution]()

[Tendency to find low-frequency solution]()

[Learning in High Dimension Always Amounts to Extrapolation](https://arxiv.org/abs/2110.09485): 

[Deep Learning without Poor Local Minima](https://proceedings.neurips.cc/paper/2016/hash/f2fc990265c712c49d51a18a32b39f0c-Abstract.html): 

## Does neural network memorize the training data?

## What happens when you scale up the neural network?

[Scaling Law from dimensionality of the data](https://arxiv.org/abs/2004.10802): $\alpha \sim 4/d$, where $d$ is dimensionality of the data. This is a very interesting result, as it shows that the scaling constant of neural network has a fascinating connection with the intrinsic property of the data.

[Pruning Data to improve scaling](https://arxiv.org/abs/2206.14486): Quality of the data matters, even in the large-scale setting! 

[Scaling Reward Model](https://arxiv.org/abs/2210.10760) : Reward modeling + RL is a promising approach in the field of deep learning, popularized by famous [chatGPT (instructGPT)](https://arxiv.org/abs/2203.02155). Scaling helps, and we should limit the KL divergence during optimization.

[Ensemble instead of scaling?]()

## Batchsize and Learning rate: what you should know about them

[In-batch variance : smaller the better?](https://arxiv.org/abs/2105.13343)

[How large should your batch be?](https://arxiv.org/abs/1812.06162)

[Larger batch size, larger learning rate?](https://arxiv.org/abs/1706.02677)

[Emergent Capabilities vs Inverse scaling]() :

## Fascinating Aspects of Neural Network

[Shortcut learning](https://arxiv.org/abs/2004.07780), [Gradient Starvation](https://arxiv.org/abs/2011.09468)
 : Neural network tends to "cheat in learning" when it has the chance. 

[Dataset Distillation](https://arxiv.org/abs/1811.10959) : Did you know that you can reversely *train the dataset*, so that neural network can learn faster? The field has grown very much.

[Localization and Edit](https://arxiv.org/abs/2202.05262) : Maybe this is too limited, but the way they do *causal tracing* to find which layer is responsible for certain output is very generally applicable.

[Information Bottleneck]() :

[Double Descent]() :

[Grokking]() :

[Bootstrapping, self-distillation, ensemble... Learning from itself? How does that even make sense?](https://arxiv.org/abs/2012.09816) :

[Adversarial Examples Are Not Bugs, They Are Features](https://arxiv.org/abs/1905.02175):

[Lottery ticket hypothesis](https://arxiv.org/abs/1803.03635):

[Neural Collapse]():

## These might provide some alternative insights

[Infinite width Neural Networks]() : Of course, we see that neural network works well in practice especially in the large-scale setting. But since their analytical training dynamics are clearly intractable, we can't really say much about them. Instead, *infinite width* neural networks are much easier to work with. [NNGP](https://arxiv.org/abs/1711.00165), [NTK](https://proceedings.neurips.cc/paper/2018/hash/5a4be1fa34e62bb8a6ec6b91d2462f5a-Abstract.html), and [Tensor Programs](https://thegregyang.com/) are some of the most fundamental papers in this field. It maybe bit too math heavy, I recommend you to read [this blog by Lilian Weng (as always)](https://lilianweng.github.io/posts/2022-09-08-ntk/) first.

[Infinite Matrix Factorizations]() : Alternatively, training dynamics of matrix factorization actually give you a very good grasp of what *might* be happening in the neural network.

[Neural ODE]() 

[Diffusion & Score Matching]()

[Common variable trick (I made this term up)]():

[Reparameterizations]():

[Gradient estimation]():

Mechanistic interpretability ([CNN](https://distill.pub/2020/circuits/), [Transformer](https://transformer-circuits.pub/)):

## Specific to Reinforcement Learning

[Why not just, learn from expert data?](https://arxiv.org/abs/2204.05618)

[Do we really need deep learning for RL?]()

[Features of the MLP is not that great when it comes to RL]()
