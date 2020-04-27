

# Midterm 2 MENG602/438
Date: April 30th 2020
Time: 5:45pm - 11:45pm

## Student's information
 
<form id="percentageBiz" method="post">
<input type="text" id="name" placeholder = "Name">
<input type="text" id="nyitid" placeholder = "NYIT ID">
<input type="submit" onclick="return getp()" value="Generate Parameters"><br>
</form>
<br>
The question is for student: 
<div id="display" style="height: 25px; width: 100%; font-weight: bold;"></div>
<br>

<script>
function getp(){
    const nameValue = document.forms["percentageBiz"]["name"].value;
    const nyitIdValue = document.forms["percentageBiz"]["nyitid"].value;
    const b = parseInt(nyitIdValue[5])+3;
    const c = parseInt(nyitIdValue[4]);
    var d = 
    document.getElementById("display").innerHTML = nameValue
    document.getElementById("display1_1").innerHTML = [1/b, 1/(b-1), 1/(b-2)];
    document.getElementById("display1_2").innerHTML = [1/(1+b), 1/b, 1/(b-1)];
    document.getElementById("display1_3").innerHTML = [1/(2+b), 1/(b+1), 1/b];
    document.getElementById("display1_4").innerHTML = [1, 1, 1];
    document.getElementById("display2_1").innerHTML = 1+b/10;
    document.getElementById("display2_2").innerHTML = 1+c/10;
    document.getElementById("display3_1").innerHTML = 1+b%4;
    document.getElementById("display3_2").innerHTML = 1+c%4;
    return false
}
</script>

## Problem 1 
A set of simultaneous linear algebraic equations results: **A** x **c** = **b**<br>

**A** = [<span id="display1_1" ></span><br>
<span id="display1_2" ></span><br>
<span id="display1_3" ></span>]
<br>
**b** = [<span id="display1_4" ></span>]<sup>T</sup>
<br>

(i)	Find the inverse matrix **A<sup>-1</sup>**.<br>
(ii)	Find Euclidean norm of **A** and **A<sup>-1</sup>**<br>
(iii)	Calculate matrix condition number using Euclidean norms, and aslo determine how many suspect digits would be needed by solving this system for minimizing roundoff errors.<br>

## Problem 2 
Determine the solution of the simultaneous nonlinear equations<br>

![alt text](Images/eq1.png "eq1")

Use Newton-Raphson method and employ initial guesses of <br>
_**x<sub>1</sub>**_ = <span id="display2_1" ></span><br>

_**x<sub>2</sub>**_ = <span id="display2_2" ></span><br>

(i) Write and calculate Jacobian matrix. <br>
(ii) Calculate x<sub>1</sub> and x<sub>2</sub> after first iteration and calculate _f<sub>1</sub>_ and _f<sub>2</sub>_ with updated x<sub>1</sub>, x<sub>2</sub>.<br>
(iii) Calcualte error of approximation (ea). <br>

## Problem 3
Application of Eigenvalues and Eigenvectors
![alt text](Images/floor1.png "fr1")
Consider the mass spring model to gain insight into the dynamics of structures under the influence of disturbances such as earthquakes.
Above figure shows such a model for a two-stroy building. Each floor mass is represented by m<sub>i</sub>, and each floor stiffness is represented by k. <br>
The frequencies for the mass vibrations can be determined by solving for the eigenvalues and by applying _MX<sup>"</sup>_ + _kX_ = 0, which yields

![alt text](Images/mx1.png "mx1")
Applying the guess **x = x<sub>0</sub>e<sup>iω<sub>n</sub>t</sup>** as a solution, we get the following matrix:
![alt text](Images/mx2.png "mx2")

where x<sub>i</sub> represent horizontal floor displacement, and ω<sub>n</sub> is the natural, or resonant, frequency (radians/s).

Let **_m<sub>1</sub>_** = **_m<sub>2</sub>_** = <span id="display3_1" ></span> (Kg)<br>
and _**k**_ = <span id="display3_2" ></span> (N/m)<br>

(i) Use eigenvalues to solve for freqencies.<br>
(ii) If m<sub>1</sub> floors is unknown, based on the observation, the frequency is 0.1, what is possible m<sub>1</sub>. 
(iii) Describe your approach to find m<sub>1</sub> by iteration method. <br>

<input type="submit" onclick="window.print()" value="Print">
## Submission
Use above print bottom to save your exam sheet to pdf and upload with your solution to **Midterm2 Submission Box** in class's blackboard. Please submit your solution before 11:45pm April 30th 2020. 

### Notice
If the the values and euqations don't match to your problem sheet, no credit will be given for this exam. 
This is an openbook exam, any tool, program, or online resource are allowed in the exam. 
<br>

<input type="text" id="pw1" placeholder="access code">
<input type="submit" onclick="return runsol()" value="Generate Solution">

<script>
function runsol(){
 alert("incorrect access code")
}
</script>
<br>

