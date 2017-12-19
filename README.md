# ML_proect_ID
Intrusion detection system using Gas pipeline dataset
This is an intrusion detection system for Industrial Control Systems(ICS). Before stating the technical details of the project, I want to list some important constraints and characteristics of ICS and ways of attacking it.
1. The attacker is not omnipotent: If the attacker can do anything, there is no point in detecting an attack. In cybersecurity we define a 'threat model' i.e. we say what is trusted and what the attacker has the power to manipulate. In this project I consider, the attacker can manipulate the network packets between the field devices and the superivisory control (SCADA). 
2. The major concern is to detect if there is an attack or not. So as a problem statement I want to increase accuracy of detecting attacks.
3. There are two reasons why we should look into simpler models to learn. 
    a. The computers on which SCADA runs in the field are very primitive. Putting a heavy algorithm will interfere with the regular functioning of the system.
    b. Generally, the tripping time of the system is very small. For example, an attacker makes SCADA believe that there is a fault in the system. So, my algorithm must detect it to be an attack before the tripping procedure is started. 
    
To have a holistic understanding of the project, it is better to read the report first. The report justifies the motivation and also gives usecase scenarios where such an attack is possible. Then it enlists all the attacks that I am trying to detect. The code is also explained in the report.
Dataset:
http://www.ece.uah.edu/~thm0009/icsdatasets/IanArffDataset.arff
