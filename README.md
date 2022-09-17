# VR electroncis and Arduino simulator


*wait for the source code to be uploaded, for whoeve want to contribute on this project, to make a full Arduino simulator in VR*




name: **salma**



## Electronics Lab

#### Summary



play with components to assemble your own electronics circuit, and will have your circuit simulated in VR



- **experience's goal**

  - being able to understand electronics better by simulating your own circuits and seeing the behavior of each component 

    

- **intended feeling**

  - curiosity about trying different circuits combinations to see what happens

  - eagerness to learn about each component behavior

    



#### Scenes

- **main scene**

  - lab containing all your components to grab it and start snapping them together

  

![](media\scifiLab1.PNG")

![](media\scifiLab2.PNG")



#### Controls and interactions

- **grabbing objects**

- **Left/Right IndexTrigger** -> snap
- **A** -> Information about each component (volt, current, status, ..) 
- **B** -> simulate
- **X ** -> Open Drawers / inventory
- **Y** -> delete object



#### Themes

- **sci-fi lab theme**
- **technical probes** like computers and screens



#### Graphics

- vibrant colors for a tech lab 
- glowing effects 



#### Prefabs

- electronics components -> resistors / capacitors / wires / ....
- drawers (inventories)
- decorations



![](E:\courses\ACC_VR_Diploma\documentation_videos_your_work\graduationProject\pictures\components.PNG)





#### Audios

- snap sound

  

#### Important Systems

- **inventory system** (drawers) for components containing infinite number of component game object spawned when slot is selected

  ![](E:\courses\ACC_VR_Diploma\documentation_videos_your_work\graduationProject\pictures\drawers.PNG)

  

  

- **connections checking system**

  *when you finish connecting your circuit, and enter **simulation mode, ** a group of scripts will check your connections (closed / open , polarity and components) to simulate your circuit

  - **in simulation mode**:
    - your circuit will be simulated and components connected will display certain behavior according to circuit
    - you **cannot** grab new objects from inventory
    - all **unconnected component** (from both sides) will disappear , and reappear again when you exit simulation mode
    - **burnt off **components (like leds) will remain in the scene (even if it is not connected from both sides), so you can easily identify and delete it later
    - you **can** grab components in simulation mode and move your circuit around, but you **cannot** grab wires and disconnect it from circuit
    - you **cannot** delete objects in simulation mode


![](E:\courses\ACC_VR_Diploma\documentation_videos_your_work\graduationProject\pictures\led_resistor_connectionCheck.PNG)



![](E:\courses\ACC_VR_Diploma\documentation_videos_your_work\graduationProject\pictures\multipleLedsConnected.PNG)





#### WorkFlow

1. choose your components from inventory, by stand in front of inventory and press **(x)** and grab them by (**hand trigger**)



2. connect your component by wire (by snapping wire terminal using **Right Index trigger**)



3. when you finish your connections, press **(B)** to enter simulation mode



4. in simulation mode, there are three options:
   - circuit won't work because of open circuit or wrong polarity
   - circuit will work but components will burn because of over voltage if you didn't use the right resistor value
   - circuit will work if your connections are right and your have your right values connected



#### important constants

- **battery (9v)**

  - volt: 9v
  - current : 20 mA

  

- **resistors**

  - available values:
    - 100 ohm (brown black brown gold)
    - 10 kohm (brown back orange gold)
    - 330 ohm (orange orange brown gold)
    - 390 ohm (orange white brown gold)

  

- **leds ratings**

  - operating volt : 1.1 v
  - operating current: 20 mA
  - available colors (white, red, blue, green, yellow, white)

  

  

  




