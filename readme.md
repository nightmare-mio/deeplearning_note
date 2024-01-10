# 本文用于记录深度学习算法有哪些已经我在深度学习过程中的一些体会总结等

# 深度学习算法

## Generative Adversarial Networks(对抗神经网络算法)(简写:GAN)
> 由生成网络与判别网络构成

## Diffusion models(扩散模型)
> 将噪声添加到数据中，通过学习噪声的逆向扩散过程进行采集数据。
### Denoising Diffusion Probabilistic Models(去噪扩散概率模型)(简写:DDPM)
> 从数据中得到图像，并逐步添加噪声。然后训练一个模型来预测每一步的噪声，并使用该模型生成图像。
### Denoising Diffusion Implicit Models(去噪扩散隐式模型)(简写:DDIM)
>
