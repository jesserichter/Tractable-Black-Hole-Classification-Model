# Black Hole Classifier
![image](https://user-images.githubusercontent.com/71369943/130124315-7369065a-c0eb-4a3b-a54b-ad96f00d2741.png)

A Machine Learning model made using Python with various ML technologies specially made for recognizing different types of Black Holes:
- Stellar Black Holes
- SuperMassive Black Holes
- Intermediate Black Hole

## Technologies Used In it
- Python
- TensorFlow
- TensorFlow.Js
- TF Lite
- Docker
- Keras
- Coral



## Usage 

You just need to make a "classifier" directory with a directory "data" inside it with all your images
For example
```
 [any_path]/my_own_classifier/
 [any_path]/my_own_classifier/data
 [any_path]/my_own_classifier/data/stellar-blackholes
 [any_path]/my_own_classifier/data/supermassive-blackholes
 [any_path]/my_own_classifier/data/intermediate-blackholes
```
 and then put your image on it. 
 This "classifier" directory will have your samples but also trained classifier after execution of "train.sh". 

## Train process
 
Just type
```
 ./train.sh [any_path]/my_own_classifier
``` 
And it will do anything for you !

## Guess process

Just type for a single guess
```
 ./guess.sh [any_path]/my_own_classifier /yourfile.jpg
```

To guess an entire directory
```
./guessDir.sh [any_path]/classifier [any_path]/srcDir [any_path]/destDir
```

## Example Result [ TF (simple TF)]
```
# ./guess.sh /synced/tensor-lib/moto-classifier/ /synced/imagesToTest/moto21.jpg
moto (score = 0.88331)
car (score = 0.11669)
```

