# The Robot Utility
author: catalin

levels:

  - basic

type: normal

category: feature

links:

  - >-
    [www.developer.com](http://www.developer.com/java/other/article.php/2212401/Introduction-to-the-Java-Robot-Class-in-Java.htm){website}

  - >-
    [www.java-tips.org](http://www.java-tips.org/java-se-tips-100019/21-java-awt/1758-how-to-use-robot-class-in-java.html){website}

---
## Content

`Java.awt.Robot` is a class used to mimic the human behavior, taking control over the mouse and keyboard. For example:

```java
Robot myRobot = new Robot();
```
Moving the mouse:

```java
myrobot.mouseMove(x,y);
//(0,0) represents the upper-right corner```
Inserting a delay:
```java
myRobot.delay(2000);
```
Pressing the left mouse button:
```java
myRobot.mousePress(
InputEvent.BUTTON1_MASK);
```
Releasing the left mouse button:
```java
myRobot.mouseRelease(
InputEvent.BUTTON1_MASK);
```
Typing a letter:
```java
myRobot.keyPress(KeyEvent.VK_H);
//types letter H
```
Note that `Robot` class won't just generate the events, but actually perform the actions. 

Some platforms will require special privileges so make sure you use `Robot` in a
```java
try {
 // use myRobot...
} catch(AWTException awe) {
 // handle exception...
}
```
block.

---
## Practice

Press the left mouse button using the `Robot`  class:
```
Robot robot = new Robot();
robot.???(
    InputEvent.???);
```
*`mousePress` 
*`BUTTON1_MASK` 
*`BUTTON2_MASK` 
*`mouseRelease` 
*`keyPress`

---
## Revision

Using the `Robot` class, move the mouse to the desired coordinates:
```
Robot myRobot = new Robot();
myRobot.???(0,0);
```

*`mouseMove` 
*`moveMouse` 
*`mousePress` 
*`mouseRelease`