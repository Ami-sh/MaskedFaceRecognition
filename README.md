#MaskedFaceVerification
In this project, we verify masked and unmasked image of a person 'X', and return true if succesfully verified, false otherwise. We basically superimpose a constant lower half image of a face on both the masked and unmasked image of person 'X' and then use the models from deepface to verify. It works decently for images with straight faces but for titled faces, not so well.

Problems with the model:

Masked-face detection model is heavily undertrained.
What can be done to improve the results? (things that we could have done and should have done to improve the results)

Tuning the threshold values using algorithms like gradient descent.
Using multiple models from deepface and taking some sort of average distance.
Instead of forced superimposition of a constant image, we can detect the facial features and the superimpose accordingly.
Use multiple lower-half images instead of one constant image.
Should have calculated accuracies, precisiion and stuff...
