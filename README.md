# Sign-to-text-language-conversion-

--SETUP BEFORE EXECUTING PROGRAM--

1. Python Version - 3.8.5

Make sure this python version is installed and the environmental variables are set properly. If the environmental variables are not set properly
you will face issues in using pip commands and python commands in further process of this project.



2. Open command prompt - Load the directory of this project code file.

Code - cd C:\Users\Downloads\Sign-language-to-text-conversion\code

This example command will open the directory of the file in the command prompt. Replace the path of the file and use the same command given above
to load the directory of this project.



3. Make sure you upgrade the pip to the lastest version. Pip won't be in the latest version as the python version is a bit depreciated version.

Code - pip install --upgrade pip
    


4. Once the pip is upgraded download the dependencies required for the project. The dependencies are given in Install_Packages_gpu.txt and Install_Packages.txt.

Code 1 - pip install Install_Packages.txt
Code 2 - pip install Install_Packages_gpu.txt



Incase if you face any errors while installing the dependencies use chrome to find out the error and rectify it. From the developer side we will
make sure that no errors shall be faced by the user.

5. Once all the dependencies are installed successfully we can start the process of running the programs one by and one.




--PROGRAM EXECUTION--

1. Run `set_hand_histogram.py` to set the hand histogram for creating gestures. 

Code - python3 set_hand_histogram.py

Use the keys 'C' - Open thresh window, 'S' - To capture the image.



2. Run `create_gestures.py` to capture gestures and save it.

Code - python3 create_gestures.py

Use the keys 'C', 'S', 'Space' to capture and pause the capturing of the images. 500 images will be captured during this process. Once all the 500
pictures are captured the program ends.



3. Run `Rotate_images.py` to rotate the images which have been captured during the create_gestures process.

Code - python3 Rotate_images.py

This process flips and rotate all the captured images so that different variations of the images can be used for sign to text conversion process.



4. Run `load_images.py` to split all the captured gestures into training, validation and test set.

Code - python3 load_images.py

This process loads the gesture images which have been captured in to training, validation and test set. So that they can all be generated into codes.



5. Run `display_gestures.py` to display all the gestures which have been captured.

Code - python3 display_gestures.py



6. Run `cnn_model_train.py` to train the model using keras.

Code - python3 cnn_model_train.py



7. Run `final.py` which gives the output window for Sign language recognition and text conversion.

Code - python3 final.py
