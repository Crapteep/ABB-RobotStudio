# Char drawing

<sup align = "left"> 
  
   *Status: The project is finished with the possibility of its further development*
  
</sup>

<p>
A simple program for drawing/engraving/laser cutting with an industrial robot. Created in ABB RobotStudio.
</p>

## List of contents
1. [Project description](#project-description)
2. [More about `config.txt` file](#More-about-`config.txt`-file)
3. [How to open project](#How-to-open-project)
4. [How to install](#how-to-install)
5. [Ideas to develop](#Ideas-to-develop)
6. [Screenshots](#Screenshots)

## Project description
The project was entirely created using ABB RobotStudio with RobotWare v6.13.03.
<p></p>

 The aim of the project is a program that allows you to engrave, write or laser cut (depending on the selected tool) any text consisting of only letters using an ABB industrial robot.
 For this purpose, a text file `config.txt` has been created, from which information about the size of the workplace and text that we want to make are read.
  <p></p>
 The number of characters are limited and depends on the size of the workplace. Of course, a minimum and maximum workplace size has been introduced, so that the text is always within reach of the robot.
 Additionally, words that do not fit in the line are automatically separated.

## More about `config.txt` file.
- Odd-numbered lines are responsible for the size of the workplace where our text is made. It must look like this: <b> 1400x800 </b>
- The even lines should contain the text that our robot is to perform.
- Each pair of lines is responsible for the execution of the text on one element. Each subsequent pair means the execution of an inscription on the next element.

## How to open project
1. Download `MG_Projekt.rspag` and `config.txt`
2. Open `MG_Projekt.rspag` with RobotStudio
3. In the M_Gieraa controller in RAPID in the 4th line, change the path to the configuration file `config.txt`
4. Start simulation.

## Ideas to develop
- adding more characters (letters, numbers, special characters)
- A query to the operator so that he can choose the number of elements to be made or whether one inscription will be made on all elements.
- Adding characters that would start typing with a new line
- Notification of finished work
- Adding security in the form of stopping the robot's work when the door is opened, an unexpected error occurs or the safety button is pressed

## Screenshots

![App Screenshot](https://raw.githubusercontent.com/Crapteep/ABB-RobotStudio/main/views/view1.jpg)
![App Screenshot](https://raw.githubusercontent.com/Crapteep/ABB-RobotStudio/main/views/view2.jpg)
![App Screenshot](https://raw.githubusercontent.com/Crapteep/ABB-RobotStudio/main/views/view3.jpg)
