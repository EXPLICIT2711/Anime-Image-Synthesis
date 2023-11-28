# Anime-Image-Synthesis
Generatibg high quality anime images using advanced Advesarial neural networks (VQGAN).

# Vector-Quantized-Generative-Adversarial-Networks-

Train VQGAN on your own data: 
Training First Stage

    1.Set path to dataset in training_vqgan.py
    2.python training_vqgan.py

Training Second Stage

    1.Set path to dataset in training_transformer.py
    2.python training_transformer.py


# Vector Quantized Generative Adversial Networks(VQGAN)  =  Variational AutoEncoder(VAE) + Generative Adaversarial Networks (GAN) 

1. AutoEncoder:

     ![image](./assets/279442786-885dfded-f17c-4a17-8af3-75e0120cb2f9.png)

    # Problems in AE
    1) Similar images are not similar in latent space(vice versa)
    2) Latent points can widely spread (no supervision)
                          

2. Variational AutoEncoder:

   ![image](./assets/279443583-ff3c6628-10ce-482f-a5fc-869aa206b5d2.png)

   # Why VAE?

   Reparametrize latent space:  make it continuous and center it around the origin

3. Vector Quantized Variational AutoEncoder:

   ![image](./assets/279446436-eccb6b55-6470-4028-9776-4f4a7107ec2e.png)

   # Why VQ-VAE?

   Applying some sort of clustering in latent space: Easier reconstruction(focus on less playful inputs) and More control over generation


 4. Vector Quantized Generative Adversial Network:

    ![image](./assets/279448279-c05ef9e4-b2e4-42a0-995b-a66911a22a42.png)

    # Why VQ-GAN?

    Better results (Adversarial loss make the results less blurry)
