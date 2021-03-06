# IEEE-hackathon-qiskit-runtime

In this project i want to use variational quantum circuit within the variational quantum eigensolver method implemented in qiskit runtime to investigate the potential energy surface (PES) of a water molecule because it is a noncolinear molecule so the bond angle of H-O-H is different than 180. To simulate this process i first create a 3D potential energy surface by varying the the angle and O-H bond distance using the result from exact diagnoalization using Numpy. The optimal angle and bond distance are determined by minimizing the potential energy surface function. Using the predicted optimal bond angles and bond lengths, we used VQE method with a customized ansatz to determine the minimal energy. Using qiskit runtime, the VQE process was run numerous times till the VQE energy is within 4 mHa of the minimal energy obtained from exact diagnolization to determine the optimal angle for the PES calculation using VQE. After the chemical accuracy is satisfied, we calculated the potential energy surface of water by varying the bond angles using VQE with the initial starting angle obtained from the previous VQE run.

The notebook was compiled on the IBMQ environment using the following modules:

qiskit-0.29

qiskit-nature

sckit-learn

qiskit-runtime

matplotlib

numpy

Disclaimer:
This communication contains general information only, and none of Deloitte Touche Tohmatsu Limited (“DTTL”), its global network of member firms or their related entities (collectively, the “Deloitte organization”) is, by means of this communication, rendering professional advice or services. Before making any decision or taking any action that may affect your finances or your business, you should consult a qualified professional adviser. No representations, warranties or undertakings (express or implied) are given as to the accuracy or completeness of the information in this communication, and none of DTTL, its member firms, related entities, employees or agents shall be liable or responsible for any loss or damage whatsoever arising directly or indirectly in connection with any person relying on this communication. DTTL and each of its member firms, and their
