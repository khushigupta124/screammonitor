ScreamMonitor: AI for Crime Prevention-

In today’s world, ensuring public safety requires innovative solutions that leverage technology for rapid threat detection and response. Traditional surveillance systems rely heavily on visual cues, often overlooking auditory indicators like screams, which are critical in signaling emergencies. This project addresses this gap by creating a system that can detect and analyze human screams in real time, offering timely alerts to emergency responders or law enforcement personnel. By integrating machine learning and advanced sound recognition techniques, the project aims to redefine security frameworks, making them more responsive and effective in preventing crimes and safeguarding individuals.
The primary objectives of this project are:
1.Real-time Scream Detection and Emergency Alerts The system aims to identify human screams instantly, triggering immediate notifications to law enforcement or emergency responders. This capability is vital for preventing violent incidents, aiding victims in distress, or mitigating risks in environments such as public spaces, educational institutions, and high-crime neighborhoods.
2.Minimizing False Alarms Through Advanced Differentiation Leveraging machine learning algorithms, the system will classify screams based on their context—such as distress versus excitement—thereby reducing false alarms. This ensures that alerts are generated only for genuine threats, enhancing the reliability and credibility of the system.
3.Integration with Broader Safety Frameworks The project envisions incorporating the scream detection system into larger safety infrastructures, including smart surveillance systems, mobile apps, and emergency response networks. Features like location-based monitoring and real-time data analysis will further enhance its utility by enabling targeted and localized safety measures.
4.Scalable and Global Safety Solution Designed to be scalable and versatile, the system can adapt to a wide range of environments, from urban centers and parks to transportation hubs and residential areas. Over time, it can evolve into a comprehensive crime prevention tool, offering customized safety solutions tailored to the unique needs of different regions and communities worldwide.

Methodology-
1.Data Collection
This project uses a carefully curated dataset divided into two categories:
Positive Class: Contains around 2000 human scream audio samples. These represent distress or emergency situations.
Negative Class: Consists of 3000 non-scream sounds which helps the model learn to differentiate between screams and regular environmental sounds.
The dataset is sourced from various platforms like freesoundeffects.com, ensuring a diverse range of audio samples for robust training.

2.Extraction of MFCCs
The next step involves extracting Mel Frequency Cepstral Coefficients (MFCCs) from the audio dataset using the Librosa library in Python.
MFCCs capture the power spectrum of sounds, effectively reducing noise and focusing on human voice frequencies. The extracted MFCC features are stored in CSV files for further analysis. MFCCs provide a more compact and informative representation of the audio, helping the model better understand the unique characteristics of human screams.

3.Training the SVM Model-
Support Vector Machine (SVM) is trained on extracted MFCCs.The model learns to classify sounds like noise, speech, shout, and scream. Once training is complete, the model is saved using
TensorFlow.

4.Training the MPN Model-
Multilayer Perceptron Neural Network (MPN) is trained over sounds present in the same dataset. It is used to further improve accuracy, learning deeper patterns in the audio.
The MPN model employs a feedforward network with multiple layers to make more complex decisions based on sound inputs. After the training process, the model is saved in TensorFlow.
The working diagram of MPN is given below.
