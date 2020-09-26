# Realtime Semantic Segmentation
It is a web application that helps us to segment the objects in real world and helps us to classify the objects.

### Description:
This project includes the segmentation and classification of  objects in real time using a web app . It helps us to identify the objects based on the color code that is assigned and helps us to identify the objects using the help of DeepLearning and Machine Learning techniques.

### Dataset:
This project is based on the PASCAL VOC 2012 DATASET [link](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar).The dataset involves 21 classes where 20 classes refer to various objects and the remaining referring to the background.Each class is assigned an unique color.

The classes in the project include:

>Person

>Bird, cat, cow, dog, horse, sheep

>Aeroplane, bicycle, boat, bus, car, motorbike, train

>Bottle, chair, dining table, potted plant, sofa, tv/ monitor

>Background

![alt text](https://github.com/ShapeAI/realtime-semantic-segmentation/blob/master/public/images/voccmap.png "Classes")


In this project we have used the weights of  pretrained model (PSPNet). It has been converted into a set of model.json and a group of sharable bin files(4 files).

Refer to this [documentation](https://huningxin.github.io/tfjs-converter/).

### Technologies Used:
1.React JS

2.HTML

3.CSS

4.ML and DL(model)

5.Tensorflow.js 
[refer](https://www.tensorflow.org/js)



### Steps to run the code:
1.First install node.js [link](https://nodejs.org/dist/v12.18.3/node-v12.18.3-x64.msi)

2.Then install npm by running [npm install]

3.Then create a react app by typing [npx create-react-app my-app]

4.Move to that repository by [cd my-app]

5.Then check if all are set up by runnning [npm start]

6.Clone this repository to your pc/laptop

7.Open a suitable editor such as VSCode,Atom,etc which is preferred to you.

8.Copy all the files according to the file structure shown below:

![alt text](https://github.com/ShapeAI/realtime-semantic-segmentation/blob/master/Hierarchy%20files.JPG "Hierarchy structure")

9.Then install the dependencies of tensorflow js:
[npm install @tensorflow/tfjs]
[npm-install http-server -g]

10.Then open the folder where the weights folder is there and open cmd and type [http-server -c1 --cors]

Once the command is executed the model is ready to be served to the tensorflow.js file  at http://127.0.0.1:8080.

11.Enter [npm start] in the terminal.

It opens a localhost with default port of 3000 where it runs our program.


### Camera options:
At default the program uses either the frontcamera or webcam of the laptop.

We can use the rear camera by changing the facingMode in video constraints of the src/index.js file

Update:

>facingMode:"environment" 

(Replace user by environment for rear camera)

>Rearcamera-"environment" Frontcamera/webcam="user"

### Deployment:

For this project I have used ngrok for deployment where it forwards the localhost to live on net until the localhost is on.

Download this software [Ngrok](https://ngrok.com/download) and follow the first 3 steps on the page to set up the software. Next, while leaving your existing command prompt that is running npm start on, start another command prompt and enter the following:


>Run the code on cmd while in the directory that has ngrok.exe

>ngrok http 3000


Link to the existing project:[link](http://a81af381c92d.ngrok.io)

Give access to your chrome website by going to this [link](chrome://flags/)

Enable the Insecure origins treated as secure and copy the link of the website to the text area and relaunch and then open chrome again and then give camera access and run the website and explore.

To check out in heroku try:[link](https://realtime-semantic-segmentor.herokuapp.com/)

(But its still in developing side but the ui and operations works whereas the segmentation map doesnt works.)

## Contributors:
### KARTHIKEYAN JM 
![alt text](https://github.com/ShapeAI/realtime-semantic-segmentation/blob/master/50882125.png "Contributor")

### SHAPE AI
![alt text](https://github.com/ShapeAI/realtime-semantic-segmentation/blob/master/69104283.jfif "Contributor")



## Note:
It is better to switch [use hardware accleration] option in google chrome settings to run if webgl is not running at normal chrome browser.

  






