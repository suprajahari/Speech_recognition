# Speech_recognition
Creating deep learning model to predict the audio commands by using Librosa and tensorflow.

### Things to learn before step into speech recognition:

  1) what is sample rate?
  2) what is time domain and frequency domain?
  3) what is mono and stereo?
  4) what is ceptral
  5) what is Mel frequency ceptral coefficient
  6) how to use Librosa and why should I use Librosa over scipy
  7) how to use tensorflow.keras to create deep learning models
  8) what is actiavtion function in neural networks?
  9) what is optimizer and loss function in neural networks?
  10) what is binary class and multiclass classification?


I created the Deep learning model using tensorflow with two layers using relu and softmax activation function. I get the audio file using glob function and read it using librosa.
Librosa automatically resamples the audio file into 22050Hz and create a audio data between [-1,1]. resample is a changing sample rate with required amount. 
Generally 44 KHz>= sample_rate >=8 KHz is used as a sample rate. sample rate doen't reduces the quality of the data but reduces the size of the data. 
Then we can get important data features from the mel frequency ceptral coefficient (MFCC). based on this data we developed the neural network model.


link to know about MFCC :
      https://www.youtube.com/watch?v=4_SH2nfbQZ8&t=2065s
