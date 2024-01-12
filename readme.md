# 本文用于记录深度学习算法有哪些已经我在深度学习过程中的一些体会总结等

# 深度学习算法

## Generative Adversarial Networks(对抗神经网络算法)(简写:GAN)
>+ 由生成网络与判别网络构成，需要训练两个网络，以两个网络进行对抗来达到不断学习。
### GAN with deep convolutional network(深度卷积生成对抗网络)(简写:DCGAN)
### Cycle GAN(循环生成对抗网络)(简写:DCGAN)
### Wasserstein GAN

## Diffusion models(扩散模型)
>+ 由前向过程和后向过程构成。
>+ 在前向过程中不断向图像添加噪声，使其达到高斯噪声。**在后向过程进行预测消除噪声**。
### Denoising Diffusion Probabilistic Models(去噪扩散概率模型)(简写:DDPM)
>+ 扩散过程基于马尔科夫链(图像的当前状态只与前一个状态有关)。
>+ **在前向过程中进行预测添加噪声**，使其达到完全的噪声。在后向过程中消除噪声。
### Denoising Diffusion Implicit Models(去噪扩散隐式模型)(简写:DDIM)
>+ 扩散过程为非马尔可夫链。
>+ 在DDPM模型上进行了优化，通过跳步的方式减少采样的步数，加速了采样过程。
### Latent Diffusion Models(潜在扩散模型)(简写:LDM)
>+ 引入了预训练的感知压缩模型，将高维度空间(高分辨率图像)转化成低纬度空间(低分辨率图像)，忽略掉图片中的高频信息，只保留重要、基础的一些特征。
>+ 不直接操作图像，而是在低维度的潜在空间进行操作。
### Stable Diffusion(稳定扩散)(PS并不是扩散模型)
>+ 根据文本生成对象。
>+ 使用**LDM稳定扩散模型**。
>+ 由**文本编码器/图像编码器,图像生成器,图像信息创作器**构成。


# TODO 学习过程中的一些专业术语记录，待之后进行学习了解
>+ 马尔可夫链
>+ 高斯噪声
>+ 贝叶斯公式
>+ 高斯分布
>+ 潜在空间
>+ UNet神经网络
