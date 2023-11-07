# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)

```
## Output
### 1. Generic Articulated Robot

![280904590-aa392712-2565-4e08-8ebe-4202a9072ff2](https://github.com/hariprasath5106/Movement-of-Robot-Joints/assets/111515488/bb9370e6-7ecf-4a5d-8805-7ddb9de9f1f7)

### 2. robot.driveJoints(0,0,0,0,0,0)

![280904388-7a609aec-cfe0-4b27-ac44-ffad03c4d9eb](https://github.com/hariprasath5106/Movement-of-Robot-Joints/assets/111515488/449dea70-d689-4847-b69b-73903e2321a3)

### 3. Movement of Joint1

![280904399-d16689e1-7213-4635-b956-19df1dfd856d](https://github.com/hariprasath5106/Movement-of-Robot-Joints/assets/111515488/9dd310e1-88ed-4936-a484-45a458472079)

### 3. Movement of Joint2

![280904473-23d70445-7b77-4ea2-a574-a2face030415](https://github.com/hariprasath5106/Movement-of-Robot-Joints/assets/111515488/a78b703e-f79e-413d-ad1f-c8d3a3965076)


### 3. Movement of Joint3

![280904550-9115dfe8-3ff9-4d2a-9f8f-ded43652038f](https://github.com/hariprasath5106/Movement-of-Robot-Joints/assets/111515488/1da6b34f-6081-4a09-ac00-69f3c15affad)

## Result
Thus the different robots joints are moved with the help of python list.
