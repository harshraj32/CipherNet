# CipherNet

This Project introduces the concept of data hiding in distributed machine learning system. Data hiding prevents cloud services where the machine learning models are hosted/ deployed, to access the sensitive data we upload in the form of datasets. We talk briefly about how we achieve Data hiding.  The core concepts of the project include Encryption techniques to encrypt the data, which are essential to the data hiding problem we are trying to solve. We use two popular datasets for Image recognition and classification, we encrypt the data based on the techniques we learned and train the model which in this case is a neural network. We build an architecture loosely based on the Arch net architecture of our base paper, which enables us to perform encryption methods on the data and also recognize and classify the data accordingly. With the rise in cloud server services, Encryption on the data and model will be essential for the progress of AI industry with safety, precaution and assurance that our data won’t be misused by some wrong entities.

## Design
![alt text](https://github.com/harshraj32/CipherNet/blob/main/images/abs.png?raw=true)

the above figure demonstrate the working of this project. The data flow of the project is as follows. The data is with the client and is passed to the encryption with the help of a public key, define in a scheme. With public key the data is passed to the encryption and the encryption performs homomorphic encryption to convert the data into encrypted data. This encrypted data is sent through the network to the model on the server side. This model preserves the encryption and generates the encrypted results. This encrypted result is passed down the network to the client side and at the decryption the secret key which was generated at the beginning along with the public key is used to decrypt the encrypted results and the decrypted results are sent to the client.

### Processing of the image
![alt processing of image](https://github.com/harshraj32/CipherNet/blob/main/images/processing.png?raw=true)

## Architecture
![alt arch](https://github.com/harshraj32/CipherNet/blob/main/images/architecture.jpg?raw=true)

## Output
Accuracy Plot of Mnist Base Model vs Encrypted Model

![alt mnist output](https://github.com/harshraj32/CipherNet/blob/main/images/mnist_acc.png?raw=true)

Accuracy Plot of FMnist Base Model vs Encrypted Model

![alt fmnist output](https://github.com/harshraj32/CipherNet/blob/main/images/fmnist_acc.png?raw=true)

## Results
Base Model Accuracy MNIST - 99.1% FMNIST - 89.03%

Encryption Model	Accuracy MNIST - 98.2%	FMNIST - 88.11%
