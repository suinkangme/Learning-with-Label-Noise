## Effect of Using APL(Active Passive Loss) and Dynamic Weights into Samples on Noise Label Dataset

<h3>[ Duration ]</h3>
- September 22nd, 2023 to December 18th, 2023 (2023 FALL, Concordia University)

<br>
<br>

<h3>[ Course ]</h3>
- COMP 433 : Deep Learning

<br>
<br>

<h3>[ Team ]</h3>

| NAME |
| --- | 
| Suin Kang |
| Deokyeong Kim | 

<br>

<h3>[ Description of the project ]</h3>
<p>
Developing a robust CNN model to address the challenge of learning with label noise.
</p>
<br>

<h4> | Dataset | </h4>
<p>
1. CIFAR-10 dataset (images) <br>
2. MNIST
</p>
<br>

<h4>| Noise Injection | </h4>
<p>
Add Symmetric label noise OR Asymmetric label noise
</p>
<br>


<h3> [ Two Approaches to build the Robust Model ]</h3>

<h4>| Baseline Model | </h4>
<p>
The BaselineModel is a robust CNN with convolutional, activation, and max-pooling layers that process input channels to output 32x32x8. It employs Xavier initialization to enhance training stability and mitigate gradient vanishing or exploding risks, ultimately yielding 10 output classes for CIFAR-10 categories in its final layer.  
</p>

<br>

<h3> | Approach 1. Baseline Model + APL | </h3>
<p>
   APL incorporates both Active Loss, which corrects labels for samples with noise, and Passive Loss, which performs regular training. This combination helps the model mitigate the influence of noise, maintaining high performance.
</p>
<br>

<h3> | Approach 2. Baseline Model + Dynamic Weight | </h3>
<p>
  This approach involves applying dynamic weights to samples, enabling the model to adapt sensitively to samples with high noise levels. By employing dynamic weights for specific samples, the model can focus more on samples with accurate labels while responding more sensitively to samples with considerable noise.

</p>
<br>


<h3> [ Related Literature ] </h3>
Weight initialization techniques for deep learning algorithms in remote sensing: Recent trends and future perspectives. <br>
https://arxiv.org/abs/2102.07004v1 <br><br>

Loss functions and metrics in deep learning. <br>
https://arxiv.org/abs/2307.02694 <br><br>

Normalized loss functions for deep learning with noisy labels.
https://arxiv.org/abs/2006.13554 <br> <br>

Co-teaching: Robust training of deep neural networks with extremely noisy labels.
https://arxiv.org/abs/1804.06872 <br> <br>

Learning to reweight examples for robust deep learning. <br>
https://arxiv.org/abs/1803.09050 <br><br>

