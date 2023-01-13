# Black Hole Classifier
![image](https://user-images.githubusercontent.com/71369943/130124315-7369065a-c0eb-4a3b-a54b-ad96f00d2741.png)

A Machine Learning model made using Python with various ML technologies in reference model from [Teachable Machines](https://teachablemachine.withgoogle.com/) specially made for recognizing different types of Black Holes:
- Stellar Black Holes
- SuperMassive Black Holes
- Intermediate Black Hole

**Note:** This project can be reused as per the requirement, but make sure to give respective credits ( read LICENSE for more info...)

## Technologies Used In it
- Python
- TensorFlow
- TensorFlow.Js
- TF Lite
- Docker
- Keras
- Coral

## Requirements ( TF )

* [docker](https://www.docker.com/products/docker-toolbox)

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

Use an absolute file path for classifier and images because the script dos not support relative path (volume mounting)
## Example Output ( TF.js )
![image](https://user-images.githubusercontent.com/71369943/130122772-b6369929-a636-432b-a227-e0b6b77806aa.png)
![image](https://user-images.githubusercontent.com/71369943/130122853-4d728642-7209-4d01-b2b4-04f40065e505.png)

## Resources
- [Source Code ( TF.js )](https://github.com/PulkitSinghDev/Black-Hole-Classifier/tree/main/TF.js_(source_code))
- [Source Code ( TF )](https://github.com/PulkitSinghDev/Black-Hole-Classifier/tree/main/TF_(source_code))
- [Source Code ( TF Lite )](https://github.com/PulkitSinghDev/Black-Hole-Classifier/tree/main/TF_Lite(source_code))
- [License](LICENSE)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Contributing Guidlines](CONTRIBUTING.md)


[<img alt="Buy me a Coffee Button" width=200 src="https://cdn.dribbble.com/users/439816/screenshots/3580937/1_.gif">](https://www.patreon.com/PulkitSinghDev) &nbsp; [<img alt="Buy me a Coffee Button" width=200 src="https://media1.giphy.com/media/kmIZ4lx2ZHpr5jY0W4/giphy.gif?cid=6c09b9525if4qmp1c3ez9l9eqvywiqx8o1ao47gyfp1v0c20&rid=giphy.gif&ct=s">](https://www.buymeacoffee.com/PulkitSinghDev)
