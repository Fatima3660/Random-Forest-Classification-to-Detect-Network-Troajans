# Network Behavioural Analysis Using Machine Learning Random Forest Classification To Detect Trojans

Trojans are a growing concern in todays world, since they are specialised in tricking people in showing they are a legitimate functioning software, but with their recent advancements theses Trojans can even go undetected by a Firewall and Anitvirus too.

### Main concern this code was created for: 
1) Trojans can change their functionality and codes to go undetected by most antiviruses
2) Most antiviruses uses static signaure analysis by comparing hash values of the malware detected to a large database of previously detected malware. This becomes difficult to detect Troans since even though the functionality stays the same, a slight change in code changes the hash value.
3) Trojans quickly spread the moment it is installed and ran on the device so by the time traditional antiviruses scan for this file amoung the millions of file a average user has, the Trojan will successfully execute its fucntionality.

### Main Goals to achieve in this experiment
In order to fill in the gaps of previous experiments my main goals to achieve in this experiment will be:
1) **Create a random forest machine learning classification and train and test it using python codes than WEKA or other tools**
  Most tools like WEKA have their own limitations i.e. not showing the exact steps in showing how to classify. Due to this, it limits you   to test the classifier with various parameters in order to find the best result. This experiment will be built on a random forest         classifier in order to address this gap in the literature because the majority of it lacked any theory or practical on random forest      classification when it is so easy to identify Trojans with this classification.
2) Show the step by step process of finding feature importance and mention the details of the features used
Create feature extraction from the dataset using python code than other tools 
By addressing this gap I can contribute to the improvement of the accuracy and efficiency using important features in detecting malware using machine learning algorithms. Instead of using tools like WEKA or TShark, I will most likely use a python library for calculating the feature importance and use the first 25 as my final features.
Use a real world dataset
3) Create a harmless trojan and transfer it over to Windows 10 and capture real time downloaded packets using Wireshark.
Use Wireshark captured packets to test it with the outputted trained classifier to detect trojans, 
4)Real time detection
In order to achieve this the data from wireshark will be saved as a csv file and then used as a dataset input on the trained classifier to predict any trojans. I'll try routing the packets to wireshark and automatically delivering the analysed packets to the classifier to perform a real-time detection. This will help detect trojans quicker reducing the window of opportunity for destructive acts to be developed.


### The project will be broken down into 3 sections:
1) Training and Testing the random forest algorithm using Kaggle dataset
2) Demonstration of a closed Nat Network attack on windows 10 using kali linux
3) Testing on real world dataset collected from WireShark windows 10 attack 
