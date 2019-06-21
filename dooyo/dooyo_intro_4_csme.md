
<style type="text/css">
pre {
    white-space: pre-wrap;       /* css-3 */
    white-space: -moz-pre-wrap;  /* Mozilla, since 1999 */
    white-space: -pre-wrap;      /* Opera 4-6 */
    white-space: -o-pre-wrap;    /* Opera 7 */
    word-wrap: break-word;       /* Internet Explorer 5.5+ */
}
</style>



---
# DOOYO

---------------------------------

**WRITE TIME :** 20190227

**SOME WORDS :** I recently want attend a meeting hosted by CSEM, and I received a mail from the organizer who want know what is Dooyo doing and who I am. I tried to explain the reason of attending this meeting for I like to learn the technology of SoC, Sensor and IoT. But she asked me to provide a more detail introduction for she is doubt about my technology background. OK, I do not known why they are so nervous about the attender. As I known, technology should be open, and Company should welcome anyone who like to learn and try its products. But I think this is also a good time for me to write my ideas. I have thinks a lot and discussed a lot with friends, without document. Thanks CSEM organizer for giving me the time to write down.

----------------
## About History 

**Dooyo** is a startup company created by **Alex** and **David**(me). 

Alex is a senior market expert. He has a strong background on market sales and policies with more than 15 years working experience. I am a technique man. I have decades years technique working experience, covering many fields, such as communication hardware and software, enterprise solution, mobile development and so on. I like technique things and interested in make life more easier by the help of technique. I treat myself as a Programmer, a Explorer, a Trekker, and a Creator.   

At the start time, we decided to make Independent Games. Alex and I are all like games, we like the the story, the action and the art behind it, especially fighting games. On the other side, game is a rapid developed area, not only the user experience and imagination scene, but also the technology. Many new technologies are used in game in the first, AR, VR, Gesture, Eye Tracking, Mobility, Wearable and so on. That is my interesting. I like technology, and want to use technology to change our life.    
 
 But, we have build a team during the development time since then. Our team evolves creative guys with different background. It is my pleasure to introduce some of team members here. Nalong is a our software architect, also a  technique problem solver in many areas. Wulong is a technique specialist focused on Hardware development and Driver software development, also a parent of a boy who was born after Wulong joined in Dooyo. Yiziyun is a designer for our game, and he like to see all sorts of Cartoons and Games. Kent is our artist, he like the beauty of violence and drawing roles with sprite of never give up! Of course I cannot mention all of our team members here, especially the memeber in coding, testing, operation and so on. Research and Development is always our major department.     

After the game production period, I start to realize the ability of our team. We team members are technique guys almost, we have the power of implementation, both hardware and software. And we want use our technique power to do something, to make our life more easier, to make world more beautiful. That is our truly mind after so long time of create production. We want make our steps beyond the scope of Game.     


---
## Our Mind

OK, what should we do? Our team is good at technology, especially in AI, Iot, IOTA, AR/VR, and has a strong interesting on Robot, ExoSkeleton, Automatic Driving and so on. Then I think these direction is a good start point for us to explore. 

 After attending many interviews and discussions with so many people in these field, I made some directions suitable for our team to dive deeper in the future.    

Following is a high-level concept diagram. 

![image](/media/dooyo_idea_0.png)




---
#### Machine Behavior Marketplace

Machine will be the future basement for our society. The live of people will depends on all sorts of machine, such as car, watch, phone and so on. We need keep these machines works well, then the producer need to keep track the data produced by their products. Also the owner of machine, i.e. every single person, need to keep privacy for themselves.

We want to build a marketplace for every machine to store, exchange information between each other. Other entities will be play a role on this platform. The entities can be any type of object, not limited to be human. For example, Manufacture will track there products, People will control the benefit of their machines after them is brought by him, Policy can query the data if some law issues should be solved, NGO can monitor the data and analyse it to find a better way to keep our planet. 

![image](/media/dooyo_idea_mbm_1.png)

Economics will be used to be the running rule between the entities of marketplace to exchange their data. For example, People who own a car, can decide what type of information can be find by other entities, and what price will be paid if some entity want to see more detail. 
  
What is machine mean? In our Machine Behavior Marketplace, machine is not limited to narrow types. Let think the scenario of Autonomous Driving. Many sensors are equipped in cars to get the realtime data from situation, including Camera, LiDAR, Millimetre Wave Radar, Ultrasonic Radar and so on. Their data will be treated as raw data in the view of Machine Behavior Marketplace. Another scenario is robot. Cleaning Robot is widely used by people now.      

From the technique viewpoint, there several parts is need to build the whole system. At the machine side, a embedded device should be existed to provide the bridge between the target machine and marketplace network. The embedded device communicate with network by a protocol which is defined by us but open to all world. Raw data is transferred by the protocol. At the center of marketplace system, there are devices to store the raw data which is sliced into multiply parts to reduce the total size. Other devices is used to analyse the raw data, then generate report data which is stored also in the network. The analyse rule is defined by entity who has the authority. Another device need to mention is data exchange, which is used to exchange data between entities. 

Some kinds of machine are listed in the following sections. We want to build them by our self.         


---
#### Recognition Planning Platform

Intelligent is a major part in the future machine society. Autonomous Driving, Auto Moving Robots, AGV ( Automatic Guided Vehicle ), all these sorts machine will need recognition ability by using all kinds of senors to know their situation. Then they need to make decision according to their designed target by human. The decision includes obstacle avoiding, path planning.

This is a complexity system, including software and hardware. We want to create a platform to implement all the dirty works.  

![image](/media/dooyo_idea_rpp_1.png)

Many sensors will be used by the autonomous cars to detect the situation, such as LiDAR, Camera ( Single or Dual Camera ), MillimeterWave Radar, Ultrasonic Radar and so on. Fusion recognition is need to merge all the information detected by these sensors. This is a very difficult work. Different sensor has different algorithm, LiDAR create 3D point cloud and need 3D object modeling and processing, Camera need computer vision to detect object, MillimeterWave Radar need Filter and even 3D point cloud processing. Then object detection will be done based the merged recognition information. Object will be divided into level according to their impact on the system target. For example People object has a higher level than other object such as obstacle object. Based on this object, some decision will be make to achieve the system target designed. It is called Planning. Planning is always divided into tasks, each task can be divided into a more small sub-task. Task is a more focused single mission, such as Auto Lane Assist, Traffic Signal Identification, Forward Collision Warning and so on. These tasks also have priorities. At last, a Resolution Mechanism will be used to merge all the task result and give the final output control singles. 

This process is a more general flow not only used in Autonomous Car, but also Robots and many other machine with automatic motion abilities. 

We want do design a framework to implement all the detail works. The platform has input and output interface for hardware to exchange data and control information, has software interface for arithmetic to plug and play, has api interface for human to monitor, also can be connected to Machine Behavior Marketplace. In conclusion, we will provide a hardware module for automatic machine to equip, a software stack for manufacture to program, a center cloud server for anyone to communicate.
        



---
#### Fusion Simulation Platform

Automation will be the future, but many difficulties still existed. Today AI is based on the big data. Model is trained from massive data, then the all the arguments are settled according to the relationship possibility between input and output. Then the inference will be processed during the production scenario, such as Self Driving Car, Autonomous Robot. But this methodology never knows how to treat the data not trained before. Several methods can handle this problem. One of them is adding rules defined by human. Decision will be made by mixing human rule and trained model. Another method is adding more abnormal testing use-cases and doing simulation. This way can make add more useful information into the training data, then make the model more robust. 

Our idea is to create such a mixed testing and simulation system, Fusion Simulation Platform. 
  



---
#### AR Education Platform 

AR is a amazing technology, We like to use it in education. Dooyo has been established a solid platform for the chinese school, and we can provide more function based on this platform. According to our plan, AR will be used in the scenario of class teaching between teacher and students.

Teacher can using our platform to generate 3D content. We provide multiply interactive mode, including Gesture, Voice and Mouse. We also provide a completely model creating toolset for teacher to generate their content very easily. After published, the content can be taught to student. During the processing of content explaining, multiply interactive mode will also play a very important role for teacher to explain thoroughly, such as scale, rotate, transfer, split, merge and animation. Yes, all the operation can be done by Gesture, Voice and Mouse. Student can see the content projected on a large screen or wall, and operate the content as same as teacher does. We provide camera sensors to capture the operation of teacher and student, edge computer to process the low-delay computing tasks, cloud server to process the time-senseless tasks. Also AR Education Platform will be connected to Machine Behavior Marketplace. Content Producer can spread their content without limit, read comments from others, and rewarded from the Publisher who want print content into books. This will construct a data economics system.    

 
 
---
#### STEAM Supplychain Platform

STEAM is now very popullar in China and all worlds. But there are some questions need to be handled.
1. Trainer (ie. School) do not know where to find the suitable STEAM contents.
2. Producer (ie. Lego) only get paid from Trainer after they buy the contents or materials.
3. Customer (ie. Child & Parent) pay for the Trainer instead of Producer, and get the finished STEAM product for free.  
We think that the payment business model is the key factor which block the STEAM running faster.

So we want to import a new role, Sponser, who will provide the material for the STEAM content. In the new business model, there are serveal roles to play with each other :
1. Trainer (ie. Scholl), who will use the STEAM content and material from Producer with free, then provide them to Customer;
2. Producer (ie. Lego), who will create STEAM content with material provided by Sponser;
3. Sponser (ie. Cocacola), who will provide material to Producer and will have the oppotunity of getting other product bought by the Customer;
4. Customer (ie. Child & Parent), who will get the finished STEAM product from Trainer, and maybe insterested to the other products provided by the Sponser, then buy them;
5. Platform (ie. Ourself), who will chain all the above roles together, providing a place to search, upload, download and buy the STEAM contents and materials.

![image](/media/dooyo_idea_ssp_1.png)

This is Business Model Innovation, technology plays a secondary role. But some tasks must be done if we want this model running well, such as Matching Algorithm, Big Data Analysing, Realtime Operation Tracking, Suggestion System and so on.  



---
#### Autonomous Driving HUD 

HUD (Head Up Display) is a convenience device for human, especially in the scenario of Autonomous Driving. Passengers are sitting while car is moving. Some immersing experience is more suitable for the passengers at these time.  

Our HUD device can be installed on two positions in the car space. 

One position is the bottom of front windshield. This type HUD can be used in two ways. First, it is used to project road image onto the front window. Drivers ( Or Passengers in Autonomous Driving Scenario ) will see the situation information in realtime, such as Traffic Lane, Navigation Direction, POI Information and so on. The second usage, the HUD can also show the image out of the Driver's sight, such as situation just ahead the bumper bar which can not be seen because of hidden by the Engine Cover.   

Another position is the top of every car window. This type HUD is used to project image onto the car window. Passengers will see a AR immersing picture, and interactive with the content, such as gaming, shopping and talking. Passenger also can upload their information to the screen, such as POI name and emotion feeling.  

By using our HUD, a tradition car cockpit will be transformed to a intelligent cockpit with immersing experience. Passenger will be more safe, and more happy during a long time of trip. 

This HUD will be connected to Machine Behavior Marketplace to exchanged content dynamically. 




---
#### Human Leg Exoskeleton 

Knee is a fragile part in Human body. I realised this seriously when my right knee is hurt during playing basketball. During the painful days, I really want to a Metal-Leg to make me move more quickly. 

So I want build a exoskeleton which will be equip on the human leg. This exoskeleton can providing additional supporting force when people crouching，more explosive force when people jumping. People will be more smart and stronger without changing the Knee!

This Exoskeleton will also be connected to Machine Behavior Marketplace to get the dynamic feature such as different scenario parameter adjustment.     



---
#### Motion Combination Equipment 

I like sport including trekking, bicycle, climbing and swimming. But the nature is not created by one way. Always when I ride my bicycle on a plain road happily, then there must be a hill laid before me after several minutes. Sadly I have to down the bicycle, walk while push my bicycle, then climb up and down to the other side of the hill. I really want fly across the hill!
  
So I designed a machine which can be used in several situations. The following is a concept diagram. 

From the the first look, It is like a bicycle. Yes, it is a real bicycle. I can ride it. But if I pull out some connector, then the bicycle can be transformed to a drone. The two wheels of bicycle will be used as the drone rotor. I can bind the bicycle frame to my back, and control the drone using the bicycle handle bars. Also I can make the bicycle transformed into a thruster, and push it into the water. The bicycle wheel will be used as the underwater propeller blades. I will control the motor by using the bicycle handle bars also. 

Because of the machine's usage, I named it as Motion Combination Equipment, where Combination means function combination of Bicycle, Drone And Underwater Thruster.
  

---
#### Boxing Training Robot

I like Boxing, it is a sport with courage, strategy and thinking. Current Boxing trainning can be splitted into three main parts: Warm-up, Sandbag, Fighting-to-Coach. 
        

 

---
## The Vision

We think the furture will be a world of Human and Machine, and our Human society will run above the Machine system.

So what should we do? We will make Machine to aid Human by the help of Technology.

That is our vision.


Reference website : [DOOYO 骨鱼科技]( http://www.dooyogame.com )

