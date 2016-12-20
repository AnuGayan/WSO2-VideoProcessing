# WSO2-VideoProcessing
Human Detection using openCV

To run this code in a ubuntu base machine, it should have OpenCV 2.4.13 installed with oracle java 1.8.

Install  OpenCV 2.4.13
Prerequisites 
Cmake / cmake-gui
Python-dev
Java (JAVA_HOME and java PATH should be set up) 

Install cmake-gui, python-dev, and other prerequisites.
'''
$ sudo apt-get install build-essential python-dev cmake-gui 
'''
Next, OpenCV 2.4.13 can be cloned from OpenCV github repository using following code
 $ git clone https://github.com/opencv/opencv.git

After the clone is completed move into the folder and create a new folder named build

Open a terminal and  type
$ cmake-gui 
 
In the gui, select the cloned opencv folder as the source path
Select the created build folder as the build path
Check the grouped checkbox
Then click the configure button.
After configuration finished configuration done notification will appear in cmake-gui. 

To build OpenCV with multi thread support tick the BUILD_TBB box from the BUILD drop down list and from “WITH” drop down list, select WITH_TBB. Keep other things unchanged.

Then click the generate button.
After generating complete close the cmake-gui.
Move into the build folder and run following commands
$ cd build
$ make -j8
$ sudo make install

This will install the OpenCV in to the machine.

Run the program

Clone the required project and open as a Intellij project.
