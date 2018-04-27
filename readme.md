An Automatic Music Transcription (AMT) system utilizing methods and principles from the realm of speech recognition. The dataset utilized consists of synth-generated monophonic saxophone recordings using a database of scales and jazz solos. Using a time-delay neural network trained to identify pitches based on MFCCs extracted from the recording, the system outputs probabilities of note occurrences for each frame. These are then fed into a language model using an HMM, which boosts accuracy by accounting for noisy measurements and the relative likelihoods of various sequences of pitches using a database of jazz solos. In the monophonic case, the system achieves 96.98% accuracy on all frames and a 0.87% WER. Future work remains to be done both to transcribe polyphonic recordings and to integrate the neural network with a more sophisticated language model attuned to the syntax, relative ordering of notes, and grammatical structure distinguishing music from speech.