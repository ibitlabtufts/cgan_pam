# cgan_pam
There are two deep learning networks:
Denoising U-Net
Denoising conditional GAN - Pix2Pix model with some modifications into the loss function, and dropout layers

Training dataset was captured from the Acoustic-X LED system which is different from the testing AR-PAM system.

We also used 3 non-learning traditional noise removal / signal improvement algorithms: Block Matching 3D (BM3D), Non Local Means (NLM) and Savitzky-Golay (SG)

We used two no reference image quality metrics - SNR and CNR
SNR = 20 * log(mean_ROI / std_background)
CNR = std_ROI / std_background
