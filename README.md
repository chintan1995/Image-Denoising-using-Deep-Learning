# Image-Denoising-using-Deep-Learning

In this repo I have implemented three different deep learning architectures for image denoising,
REDNet; https://arxiv.org/pdf/1606.08921.pdf
Multi-level Wavelet CNN (MWCNN); https://arxiv.org/pdf/1805.07071.pdf
PRIDNet; https://arxiv.org/pdf/1908.00273.pdf

I found that PRIDNet was giving the best results as compared to the other two, giving me the best PSNR and SSIM scores along with best visualizations which were very close to the ground truth images.

Note 1: Improvements shown below are over original pairs
Note 2: Time taken shown below is time taken to predict a single image
+-------------------------------+---------+--------+------------------+------------------+----------------------+
|             Model             |   PSNR  |  SSIM  | PSNR Improvement | SSIM improvement | Time taken (seconds) |
+-------------------------------+---------+--------+------------------+------------------+----------------------+
| Original X-y pairs (No Model) | 26.3779 | 0.6000 |        -         |        -         |          -           |
|       REDNet (Baseline)       | 30.5713 | 0.7932 |      4.1934      |      0.1932      |        ~ 4.64        |
|     MWCNN (using Wavelets)    | 32.5220 | 0.8397 |      6.1441      |      0.2397      |        ~ 2.7         |
|   PRIDNet (using Attention)   | 33.3105 | 0.8534 |      6.9326      |      0.2534      |        ~ 2.64        |
+-------------------------------+---------+--------+------------------+------------------+----------------------+
