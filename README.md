# WHS-FTC-GramGra07-Code_Training_Mod       
## Created by FTC team 10448 Mach 5
### To help incoming freshman and everyone that needs it understand the coding process and language involved in ftc programming

If something loads weird or looks like it doesn't belong, this link should work better. https://github.com/GramGra07/WHS-FTC-GramGra07-Code_Training_Module/blob/main/README.md

# Table of Contents
- [Links](#link)
- [Tips and Hints](#tip)
- [Fatal Erorrs](#fatal)
- [Getting Started](#start)
  - [Forking](#fork)
  - [Cloning the repository](#clone)
- [Github Basics](#gbasics)
  - [Commits](#commit)
  - [Push](#push)
  - [Pull/merge](#pull)
  - [Managing your server](#manage)
  - [Personal Access Token](#pat)
- [Coding](#code)
  - [Code Basics](#cbasics)
    - [What is a...](#wia)
      - [Operation](#oper)
      - [Variable](#var)
      - [Function](#func)
      - [If Statement](#if)
      - [Print/Telemetry System](#print)
      - [Loop](#loop)
      - [Import](#import)
      - [Configuration](#config)
  - [Getting Started](#start2)
  - [Setting up your files](#files)
  - [Using Variables](#usevar)
  - [TeleOp](#tele)
  - [Autonomous](#auto)
  - [Editing your code](#edit)
  - [Functions](#functions)
- [Encoders](#encode)
  - [How do they work?](#eWork)
  - [How do I use them?](#eUse)
  - [Why should I use them?](#eyUse)
- [Running your code](#run)
- [Machine Learning and TFOD](#ml)
- [Updating your devices](#update)
- [Overall game](#ovr)
- [Feedback](#feed)
- [Agknowledgements](#agk)
- [Glossary](#gloss)
- - - - - - - - - 
## Useful Links <a name="link"></a>
- My [user page][user] (GramGra07)
- FTC Official Github [user page][ftcpage]
- Team Resources [folder][team]
- [Rev Hardware Client][rhc]
- [FTC BasicOpModeLinear (21-22)][lop]
- [Game Format](#ovr)
- [Game Manual 0][gm0]
- [FTC Resource Library][lib]
- [Github -> Discord Web Hooks][web]
- [3D Printing Basics by my Dad][3D]
- - - - - 
## Tips and Hints <a name="tip"></a>
### 1. PRACTICE!!
- It is known that if you practice somthing, you will get better at it over time, this is the same for coding and robotics
### 2. Ask Questions
- The WHS team has a lot of intellegent people who would love to help you if you simply ask
### 3. If you don't know a concept, look it up
- There are a lot of helpful solutions and people on the internet, someone **WILL** usually know the answer to your problem
### 4. READ
- All of the example opModes have very helpful comments to show you exactly what each part does, also if you read this whole thing you should be good to go
### 5. Collaborate
- A lot of problems can be solved by collaboration with friends and peers
### 6. Use prior knowledge
- Even if your prior knowledge is in a different language, it **will** help you understand this code.
- - - - - - - -
## Fatal Errors <a name="fatal"></a>
When updating or upgrading your control hub, you may get an error saying something like, could not find a file, in some random folder that you can't find. This is caused by an error in your gradle code. If you can't find another way to fix it I would recommend this method, it is a little complicated but will solve it. First, create a new repository **DO NOT ADD ANYTHING AUTOMATICALLY** not even a read me we will call this repository our bridge. Then scroll down to the bottom and tap import from repository, grab the URL of your old repository and make sure it finished importing. Then go into the old repositories settings and delete the repository. Then go to the FTC Robot Controller and fork it. You will want to clone both the bridge repository and the new one we just forked. Now you will copy over all of your working files from the bridge repo and put them in your new repository. As soon as that is finished and commited you should be good to go, you can then delete the bridge repository.

## Getting started <a name="start"></a>
In order to setup your repository correctly you will do 2 things. 1. Fork and 2. Clone this will get the repository to your github account and then put that repository local on your computer. Remember **only one person will need to fork the repo** then you will share it to the rest of your team. You will go through ![settingsa][step1] and to **collaborators** then add your team members using the add people button.
  
### Forking <a name="fork"></a>
Go to this [website][ftcpage] and find the latest repository from the company. Press the ![fork button][fork] button. This will "copy" the repository onto your github account. Remember **only one person will need to fork the repo**!
  
### Cloning the repository <a name="clone"></a>
To clone the repository, first find it on your github profile. You have 2 options on what to do you can do it through android studio or through github.
**Everyone will need to do this!!**

Android Studio:
Tap ![fila][file], then ![newa][new] , ![vcsa][vcs]. Go back to your repository and copy the url, paste it into the box and make sure the destination is desktop. You might need to have an access token to do this.
  
Github:
Navigate to the repository you want to clone. Tap ![codea][code] then select ![zipa][zip]. This will download it to your computer. Extract the zip file (double click) and move it to desktop. Then, go back to Android Studio. Tap ![filea][file] then ![opena][open] and select the path where the folder is (desktop).
  
## Github basics <a name="gbasics"></a>
Github is organized in a few sections. One, the code section, this is where your code and files are stored. Your repositories, where all of your code is stored and your profile, where all of your repositories are stored.

### Commits  <a name="commit"></a>
  
Commiting is an essential part in every part of coding while connected to github, it makes sure you have the latest edited version of your code local    on your computer, we got the code local to the computer in cloning. In a github file it is a green rectangular button at the bottom of the    file that says commit changes, ![gitCommita][gitcommit] when commiting directly from github it strictly gives the code to github, you will not have the code local yet. To make your code local you will need to pull in your code app, most likely android studio. In android studio, the commit button is a check mark in your top right corner.![commita][commit] You are also allowed to commit and push, to be explained later in push. You will also need a commit message to be able to push the commit.
  
### Push <a name="push"></a>
  - What is a push?
    - A push will essentially do exactly as it says, push the code to github. This makes sure that you not only have the latest version of code locally, but also sent to github through the cloud. This is essential for working on code together as a team and collaborating. The push button is the arrow next to the commit button, it will be pointing out, where you want the code to go.![pusha][push] Commit and push does both at the same time to simplify the process. Also see pull/merge
  
### Pull/merge <a name="pull"></a>
 - What is a pull?
    - A pull is the exact opposite of a push. It will take the currennt version of the code directly from github and sync it locally to your device/coding app. This is also essential as it allows you to get the teams latest version of code. This is helpful when multiple people are working on code all at once. If you are pushing sometimes it will ask you to merge your current code, this means you dont have the latest version, not to worry though as if you say yes github will automatically merge and add your code to the latest code. The pull button is an arrow pointing in, or towards your computer. ![pulla][pull]
  
### Managing your server <a name="manage"></a>
Managing a server is really not that hard if you do it correctly from the start. There is a settings ![settingsa][setting] button in your repository, in this tab you will find a bunch of options, it is better if you don't mess with anything that you don't know what it does. In the collaborator tab you will need to add @stcline (if you are a part of WHS). Other than that there are really no settings you need to mess with except maybe email notifications if you would like that.
  

### Personal Access Token <a name="pat"></a>
In github, tap on your profile ( top right corner ), then:
  
1. ![step1a][step1]  
2. ![step2a][step2]  
3. ![step3a][step3]  
4. ![step4a][step4]  
5. ![step5a][step5]  
6. ![step6a][step6]  ( Select all, it will work better that way )

## Coding <a name="code"></a>
The java coding language that we use is not incredibly hard to learn once you figure it all out. It follows all of the coding fundamentals you may already know.

# **IMPORTANT** when editing your code, only edit it in the **teamcode** section, you will have to copy and paste the files from the external samples. **DO NOT** edit the ftc robot controller sample code
### Coding Basics <a name="cbasics"></a>
Go through this section if you have no expirence coding, if you are expirenced, skip this.
### What is a... <a name="wia"></a>
- Operation <a name = "oper"></a>

```==``` is equals

```!=``` is not equals

```<=``` less than or equal to

```>=``` greater than or equal to

```>``` greater than

```<``` less than

Math:

```++``` increments by one

```--``` decreases by one

```variable += 1``` equivelent of variable + 1 = variable

```variable /= 1``` equivelent of variable / 1 = variable

```variable -= 1``` equivelent of variable - 1 = variable

```variable *= 1``` equivelent of variable * 1 = variable


- Variable <a name="var"></a>
  
  A variable is a holder of a value, these values can be anything, as explained in Using Variables. You can use these to store values such as an on off switch, or a progress update, you can also use this as a place to store the power for motors. You will also declare your motors and servos as variables. A local variable can only be used where it was defined or set. A global variable can be used wherever. FTC doccumentation also lets us use some of their universal variables such as DcMotors and Servos, these are all imported by import statements at the begining of your code.
  
- Function <a name="func"></a>
  
  Functions are statements to make the code run one part when you "call" the function. It is like calling a whole new section of the code. This is useful to have the code execute specific instructions. This is useful to tell the code to update something or to set a value to a variable. You can also set parameters that are localized variables. A local variable can only be used in that function. Parameters are very useful to help us define and change local variables inside of of the function.
  
- If statement <a name="if"></a>
  An if statement is simply ```if (condition) { (do something) }```. Conditions can be found in [operations](#oper).
  
- Print/telemetry statement <a name="print"></a>

  Print statements are very useful in debugging your code, essentially what they do is show you a value that you tell it to. ```telemetry.addData("caption"," info")``` This will give you values on the Driver Station phone and you can use this to see values like if a certain variable is on or off. In other languages you would use ```print('',value)``` to get the same information.

- Loops <a name="loop"></a>
  
  While loops are very helpful in robot code. They can help you to make the robot do something until a condition is met. These are used by the ftc company in their own opmodes to have the robot be on when you tell it to. These are very useful for distance or color sensors. For loops run the event a certain amount of times. ```for x in range(10){```, this would have the stuff in the loop run 10 times.
  
### Getting started <a name="start2"></a>
- General Knowledge
  - ```;``` must be at the end of every line except if it ends in ```{``` or ```}```
  - ```{``` is used to begin the code for the function, ```}``` ends the function

- Configuration <a name = "config"></a>

```DcMotor name = hardwareMap.get(DistanceSensor.class, "name");```
 
The second name is the one you will use in the configuration guide in your driver station. The first name is the one you will use to set powers and other functions.

### Setting up your files <a name="files"></a>
Refer to the blank examples [TeleOp][beTele] and [Auto][beAuto]. These both have the proper setup and code to get started coding both of these modes. I will get into more detail into what everything means in TeleOp and auto.

### Using variables <a name="usevar"></a>
Variables in java consist of:
```
boolean
int
double
float
String
```
- Boolean = True or False
- Int = Integer, a whole number
- Double = Floating point number
- Float = Decimal (up to 7 digits)
- String = Text value

Boolean is used to determine whether a value is true or not, an on/off switch
  
Int is used for a constant value like your team number, a certain value to multiple etc.
  
Double is used for your motors, this is the best method because it supports all numbers so you can use it for storing gamepad inputs.
  
Float is most commonly used to store color values
  
Strings are used to store common strings or text values like a status of initialization

- When to use public vs. private variables?
  - You generally want to always use public unless it is something that you don't want to share with other opmodes, like a runtime.
  
### TeleOp <a name="tele"></a>
Here is the [FTC BasicOpMode (21-22)][lop] it uses 2 motors.
In the [blank TeleOp Example][beTele] you will find that there are 20 lines
```
//imports
@TeleOp(name="exampleTeleOpBlank",group="Pushbot")
//@Disabled
public class exampleTeleOpBlank extends LinearOpMode {
    HardwarePushbot robot = new HardwarePushbot();
    private ElapsedTime   runtime = new ElapsedTime();
    @Override
    public void runOpMode(){
        runtime.reset();
        getRuntime();
        waitForStart();
        while (opModeIsActive()){
            getRuntime();
            telemetry.addData("Time:", String.valueOf(runtime));
        }
    }
}
  ```
First, comments are indicated by ```//```
  
Imports are how you get the references and all the different pieces to the code.
  
Next we have ```@TeleOp(name="exampleTeleOpBlank",group="Pushbot")```, this means that this opmode is being classified under the teleop section, with the name "exampleTeleOpBlank" and it is being placed in the Pushbot group
  
Now we have the ```public class exampleTeleOpBlank extends LinearOpMode{``` this means that this opmode can now be used as a base opmode, extending an opmode means that all variables and functions are shared between the opmodes. In this case the file is extending the Linear Op Mode file which you will be able to find in your forked repository.
  
Next we have our ``` HardwarePushbot robot = new HardwarePushbot(); ``` and ```private ElapsedTime   runtime = new ElapsedTime();``` the first part declares the robot as a robot, we will be using pushbot software for the season. Elapsed time is a very important thing to consider, it times the round as it is going. You can use this for a lot of things including having an endgame timer and restricting your auto time to 30 seconds.
  
Next we have the function ```public void runOpMode(){``` this runs when you press Init it will run that part. Remember, when you hit Init, it is not running the whole program yet, just the small part in between runOpMode and opModeIsActive.
  
Now we will run ```runtime.reset();``` and ```getRuntime()```, these are required in order for your runtime to be correct.
  
```waitForStart();``` tells the opmode to wait until the user presses go, when this happens, everything inside this function runs.
  
```telemetry.addData("Time:", String.valueOf(runtime));```, telemetry is your equivalent of printing data in python and other languages, using this will print onto your phone, "Time: 60(or what the time is).
  

### Autonomous <a name="auto"></a>
In the [Blank Autonomous Example][beAuto] you will find 18 lines.
```
//imports
@Autonomous(name="exampleAutoBlank", group="Autonomous")
//@Disabled
public class exampleAutoBlank extends exampleTeleOpBlank {  //your doc name *extends* your main code branch
    private ElapsedTime   runtime = new ElapsedTime();
    @Override
    public void runOpMode(){
        runtime.reset();
        getRuntime();
        waitForStart();
        //actual code
        while (getRuntime()<=30) {
            getRuntime();
            telemetry.addData(String.valueOf(runtime), "Working");
        }
    }
}
```
Imports are how you get the references and all the different pieces to the code.
  
Next we have ```@TeleOp(name="exampleAutoBlank",group="Autonomous")```, this means that this opmode is being classified under the autonomous section, with the name "exampleAutoBlank" and it is being placed in the autonomous group
  
Now we have the ```public class exampleAutoBlank extends exampleTeleOpBlank{``` this means that this opmode can now be used as a secondary opmode. In this case the file is extending the exampleTeleOpBlank file.
  
Now we don`t have to use ``` HardwarePushbot robot = new HardwarePushbot(); ``` because it has been shared through extension but we have to do ```private ElapsedTime   runtime = new ElapsedTime();``` because it is private.
  
Next we have the function ```public void runOpMode(){``` this runs when you press Init it will run that part. Remember, when you hit Init, it is not running the whole program yet, just the small part in between runOpMode and opModeIsActive.
  
Now we will run ```runtime.reset();``` and ```getRuntime()```, these are required in order for your runtime to be correct.
  
```waitForStart();``` tells the opmode to wait until the user presses go, when this happens, everything inside this function runs.
  
```while (getRuntime()<=30) {
       getRuntime();
       telemetry.addData(String.valueOf(runtime), "Working");
  }
  ```
  
This gets the runtime, checks it and if it is less than or equal to 30 seconds, it keeps running. If it is over or equal to 30, it stops.


### Editing your code <a name="edit"></a>
One major part is editing your code, to do this you will open your project in android studio, then tap FTC Robot Controller/src/main/java/org/firstinspires/ftc/robotcontroller/external/samples to get to the samples, you will need to find the teamcode part to edit your code correctly.

### Functions <a name="functions"></a>
- What is the format?
 ``` 
  public void imaginaryFunction(){
    //code
  }
  ```
- What about parameters?  
 ```
 public void imaginaryFunction2(int hi, boolean hello){
    if (hello == true){
      //do something
      int hi+=1;
    }
  }
  ```
- What about calling a function?
```
  imaginaryFunction(6,false);
```
- Returning values?
```
 public int imaginaryFunction3(int hi, boolean hello){
    if (hello == true){
      //do something
      int hi+=1;
      return hi;
    }
  }
```
You will see that this is saying public int, you use void if you are returning nothing, and the proper variable type if you are returning something. This would be called as, ```telemetry.addData("Number",String(imaginaryFunction3(9,true)))``` 
  
Hint: Int() puts the string into int form 

## Encoders <a name="encode"></a>
Encoders are very accurate measurement systems that rely on the wheel movements to measure distances.

### How do they work? <a name="eWork"></a>
![encoder demo](https://user-images.githubusercontent.com/101433010/204153129-1034463b-cef9-4044-8814-035f8cbce675.png)

Most of them work by having a light on one side of the encoder disk. On the other side of the disk there is usually a reciever. On the encoder disk there are a bunch of holes, this is the encoder ticks per revolution and you should be able to find this where you ordered the motor you are using. Most of the motors available for FTC have encoders built into them.

![encoder](https://user-images.githubusercontent.com/101433010/204154390-d6a49351-b7ba-4319-a151-6f3f3db761b1.gif)

### How do you use them? <a name="eUse"></a>
```
static final double COUNTS_PER_MOTOR_REV = your specific encoder counts per revolution;
static final double WHEEL_DIAMETER_MM = your wheel diameter in mm;
static final double WHEEL_DIAMETER_INCHES = WHEEL_DIAMETER_MM * 0.0393701;     // For figuring circumference
static final double COUNTS_PER_INCH = (COUNTS_PER_MOTOR_REV * your gear ratio) /
            (WHEEL_DIAMETER_INCHES * 3.1415);//gets the overall counts per inch to help with encoders
```
These calculations are the exact calculations that you shoud use to calculate the counts per inch of the encoder. 
```.setMode(DcMotor.RunMode.STOP_AND_RESET_ENCODER);```
This run mode will stop and reset the encoder to 0 ticks.
```.setMode(DcMotor.RunMode.RUN_USING_ENCODER);```
This run mode will make it start to track the encoder position.
```newLeftTarget = motorBackLeft.getCurrentPosition() + (int) (leftInches * COUNTS_PER_INCH);```
This sets a new target by setting a target position based on the current position.
```.setTargetPosition(newLeftTarget);```
```.setMode(DcMotor.RunMode.RUN_TO_POSITION);```
This sets the target positon of the motor to the target we just got above. It will also run the motor to the position.
After that use the method ```.setPower(1);``` to set the power of the motor.
```
while (opModeIsActive() &&
   (runtime.seconds() < timeout) &&  //timeout is used to make sure it doesn't run for too long 
   (motor.isBusy())) {

   // Display it for the driver.
   telemetry.addData("Running to", -newLeftTarget);
   telemetry.addData("Currently at", motor.getCurrentPosition());
   telemetry.update();
}
```
This will make sure it doesn't stop before going the distance it needs to. After this ```.setPower(0);``` will make the robot and wheels stop.
You need to do ```.setMode(DcMotor.RunMode.RUN_USING_ENCODER);``` again to make turn off run to position.

### Why should you use them? <a name="eyUse"></a>
You should use them because they are very helpful to go to an exact distance. Using the opmode found [here][eDemo].

## Running your code <a name="run"></a>
To put the code onto your robot, you will plug in the RC phone or the control hub to your computer and press the ![runa][run] button. It will take a bit to load and once it finishes, you can disconnect and then go to your DS phone and select your opmode, then select the run button once, tap it again and your code will run.

## Machine learning <a name="ml"></a>
In FTC we typically use machine learning an AI's to detect images. In the FTC sample code in concept tensor flow object detection or TFOD, this is exactly what this does, it uses a tensorflow lite model in order for the robot to detect certain images, FTC has already trained some of it for us, but if you want to create your own AI it will take a little bit more work. [Here is the FTC object detection software][tfodweb] To start, make sure your team is registered and you have roles set up correctly, this [website][mlset] will show you exxactly how that is possible. Note that only coaches can put video into the recognition so either arrange for a time or have your coach sign in for you *wink*. Then you will take your videos, I would recommend (for Power Play season) to have 6 videos, all 3 sides on both color cones, this will allow for the most accurate design. I just used wevideo to combine these videos into one. Once your coach or you have uploaded the video to the [Machine learning site][ml], you will have to wait for it to "extract" the frames. Then you will click on the description and get to work, you will get a picture of your video, make your object detection by dragging your box over the part you want it to detect and name it. Then click start tracking. This might take a while and you will have to watch it like a hawk. It might think some of your images are the same label in which case go to the first frame it messes up and simply change the label and hit start tracking. Once you have labeled all of your frames, you will select your video and click produce dataset, all of the default settings should be good and this is the shortest part of the process. Next you will have to select the dataset and click start training. This part will take as long as you want it to take, I would recommend 3000 steps as this will give you the highest accuracy. Once you download your model, place it into your assets folder and change ```private static final String TFOD_MODEL_ASSET = "PowerPlay.tflite";``` in your code to ```private static final String TFOD_MODEL_ASSET = "your file name.tflite";```. Now you will have to go back to the datasets and look at your labels, put these labels into the FTC sample code and you are good to go. 

- Getting a VuForia key

Go to [this website][vu] and log in, and create a new key.

Video showing entire process:

https://user-images.githubusercontent.com/101433010/199403553-69995287-3eaf-4af7-b74c-d8ae17b0868a.mp4


## Updating your devices <a name="update"></a>
Go to this [website][rhc]. It will take you to rev hardware client. Once you download the app you will be able to connect the DS phone or the Control Hub and it will show you your possible updates, take them all and you are good to go!
  
## Overall Game <a name="ovr"></a>
The game begins with a 30 second autonomous period, runtime helps us achieve this, and then a 2 minute TeleOp period, the goal is to score as many points as possible.
  
## Feedback <a name="feed"></a>
I would love to have feedback on this repository. You can contact me through the discussions! Thanks!

## Agknowledgements <a name="agk"></a>
- [Google][ggl]
- [Mr Cline][clineuser]
- [Mr Mayfield][juser]
- [FTC User Page][ftcpage]
- [Rev Robotics][rev]
- [Android Studio][aslink]
#### Proofreaders
- [Sir C Timmons][cuser]
- [Sir B Sanger][buser]

## Glossary <a name="gloss"></a>
First Tech Challenge
A repository is a folder hosted on github that contains code and items.
Push and pull at the same time using github  
A TeleOp is an opmode that uses your gamepad inputs to control your robot, it is on the right side of the phone when selecting an opmode.
A  Automonous opmode is an opmode that continuously loops for 30 seconds at the beginning of the each match, it is on the left side of the phone when selecting an opmode.
My apoligies if this doesn't work, some code software allows this exact code, some doesn't.
Some devices accept this.
Driver Station
Robot Controller
  
  
[rhc]: https://docs.revrobotics.com/rev-hardware-client/getting-started/installation-instructions
[ftcpage]: https://github.com/FIRST-Tech-Challenge
[user]: https://github.com/GramGra07
[team]: https://github.com/WindsorHSRobotics/Team_Resources
[rev]: https://www.revrobotics.com/
[clineuser]: https://github.com/stcline
[aslink]: https://developer.android.com/studio
[ggl]: https://www.google.com/
[lop]: https://github.com/FIRST-Tech-Challenge/FtcRobotController/blob/master/FtcRobotController/src/main/java/org/firstinspires/ftc/robotcontroller/external/samples/BasicOpMode_Linear.java
[cuser]: https://github.com/ctimmons25
[juser]: https://github.com/JohnMayfield
[buser]: https://github.com/sangerb19
[gm0]: https://gm0.org/en/latest/
[lib]: https://www.firstinspires.org/resource-library/ftc/game-and-season-info
[web]: https://gist.github.com/jagrosh/5b1761213e33fc5b54ec7f6379034a22
[mlguide]: https://ftc-docs.firstinspires.org/ftc_ml/
[ml]: https://ftc-ml.firstinspires.org/
[mlset]: https://ftc-docs.firstinspires.org/ftc_ml/logging_on/logging-on.html#adding-students-to-your-teams-ftc-ml-workspace
[tfodweb]: https://github.com/FIRST-Tech-Challenge/FtcRobotController/blob/master/FtcRobotController/src/main/java/org/firstinspires/ftc/robotcontroller/external/samples/ConceptTensorFlowObjectDetectionWebcam.java
[vu]: https://developer.vuforia.com/license-manager
[3D]: https://docs.google.com/presentation/d/1MeLkA9mCI4vZMiejlqMZpAhZvbV2ThvSf6oZBzhQGdo/edit?usp=sharing
  
[fork]: /images/fork.png
[gitcommit]: /images/gitCommit.png
[commit]: /images/commit.png
[push]: /images/push.png
[pull]: /images/pull.png
[run]: /images/run.png
[setting]: /images/settings.png
[beTele]: /examples/exampleTeleOpBlank
[feTele]: /examples/exampleTeleOpFull
[beAuto]: /examples/exampleAutoBlank.java
[feAuto]: /examples/exampleAutoFull.java
[code]: /images/code.png
[zip]: /images/zip.png
[vcs]: /images/vcs.png
[at]: /images/at.png
[step1]: /images/step1.png
[step2]: /images/step2.png
[step3]: /images/step3.png
[step4]: /images/step4.png
[step5]: /images/step5.png
[step6]: /images/step6.png  
[file]: /images/file.png
[open]: /images/open.png
[new]: /images/new.png  
[import]: /examples/import
[eDemo]: /examples/RobotAutoDriveByEncoder_Linear.java
