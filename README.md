# Lungzometer
Obtain the audio and through its properties of .wav we predict the patients condition as normal or abnormal lung
data set was obtained from https://www.kaggle.com/vbookshelf/respiratory-sound-database

### Problem Statement
The present pandemic COVID-19 major impact is on the lungs of the human being which reduces the 
breathing rate and oxygen intake, CT scan are best preferred by doctor to assist and identify COVID-19 stage 
or pneumonia in the people. Not only can make impact in the next pandemic but also post-pandemic situation 
this device can be able make life better with better diagnosis. This CT scan is time consuming and leads the 
individual to exposer of unwanted radiation. The health care institutions are facing a huge problem at this time 
hence to try solving we propose Lungzometer.
### Problem Solution
Hence to tackle this problem a non-invasive process has been proposed to identify the abnormalities and 
intensity of the abnormality through the analysis of sound generated in lungs. A less complex and high accurate 
model has been designed to be well suited for a tiny smart watch, smart phone or to any smart health care 
device. Stethoscope is one of the modes in which sounds generated in lungs are captured. The same technology 
in stethoscope is today embedded in smart device. The processed sound wave is analysed to extract the features 
such as Max Frequency recorded (in .wav file), the time taken for a cycle and many more. Along with-it
general info about the patient is also collected such as age, sex and patientID. The extracted feature set is fed 
as an input to our algorithm where later Lungzometer makes the diagnosis and the result is passed to patients, 
doctors and local authorities.

### Methodology
The dataset consists of 920 recording of individual patients and sound recorded from placing the stethoscope at 
different positions w.r.t lungs such as Trachea (Tc), Anterior left (Al), Anterior right (Ar), Posterior left (Pl), Posterior
right (Pr), Lateral left (Ll) and Lateral right (Lr). The dataset is a labelled data set. Data is converted into a CSV format 
containing the maximum frequency, time taken for the recording, patientID, Age and sex of the patient. Each 
recording is taken as an instance. For 920 recording 6898 observations are generated in CSV format. The primary 
focus is to determine the lung status as normal or abnormal based on the analysis of the waves or signals generated 
when the patient is breathing.
Random forest is a Supervised Machine Learning Algorithm that is used widely in Classification and Regression 
problems. It builds decision trees on different samples and takes their majority vote for classification and average in 
case of regression. One of the most important features of the Random Forest Algorithm is that it can handle the data 
set
<br />
Steps involved in random forest algorithm:<br />
Step 1: In Random Forest n number of random records are taken from the data set having k number of records.<br />
Step 2: Individual decision trees are constructed for each sample.<br />
Step 3: Each decision tree will generate an output.<br />
Step 4: Final output is considered based on Majority Voting or Averaging for Classification and regression 
respectively. <br />
The number of trees used in the forest are 5.
