# MaskedFaceVerification
In this project, we verify masked and unmasked image of a person 'X', and return true if succesfully verified, false otherwise. We basically superimpose a constant lower half image of a face on both the masked and unmasked image of person 'X' and then use the models from deepface to verify. It works decently for images with straight faces but for titled faces, not so well.

Problems with the model:
1) Masked-face detection model is heavily undertrained.

What can be done to improve the results? (things that we could have done and should have done to improve the results)
1) Tuning the threshold values using algorithms like gradient descent.
2) Using multiple models from deepface and taking some sort of average distance.
3) Instead of forced superimposition of a constant image, we can detect the facial features and the superimpose accordingly.
4) Use multiple lower-half images instead of one constant image.
5) Should have calculated accuracies, precisiion and stuff...


<img width="1014" alt="how it works?" src="https://user-images.githubusercontent.com/54100667/179431468-9645a9ea-2cae-4a10-a52c-74fd1b7d82ff.png">
