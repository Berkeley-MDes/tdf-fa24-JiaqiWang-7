# Hello DES INV 202 Student!
Welcome to your new GitHub repository! 

# Outline
[week 1](README.md#week-1)

[week 2](README.md#week-2)

[week 3](README.md#week-3)

[week 4](README.md#week-4)


[example](README.md#example-report-1)

# Week 4 #
## Week of 09/23/2024
**Personal Ecosystem Diagram:**
Apple has designed an ecosystem where each device plays a specific role, yet they all work together seamlessly to enhance the user's digital and physical environment. Here's how this ecosystem functions from my perspective:

1. Central Hub: iPhone
The iPhone serves as the heart of Apple's ecosystem. It connects to the user’s physical environment (e.g., light, sound, location) and other devices like the Apple Watch, AirPods, and CarPlay. It collects bio data (heart rate, steps, etc.) from the Apple Watch and syncs it to the cloud (iCloud) for easy access across other devices. The iPhone integrates hardware sensors (like GPS, accelerometer, and touch) and software (like health, fitness, and communication apps) to manage interactions.

2. Wearable Devices: Apple Watch and AirPods
Apple Watch collects and monitors bio data like heart rate and movement, providing health-related notifications and real-time fitness tracking.
AirPods offer seamless audio connectivity. They automatically switch between devices (iPhone, iPad, MacBook) based on user interaction, providing a hands-free experience with features like Siri integration for voice commands.
3. Environment: CarPlay, Light, and Sound
Devices like CarPlay extend the iPhone’s functionality to the car. The system interacts with the environment’s sound and light settings, enhancing convenience and safety.

4. iCloud: Data Sync and Continuity
iCloud ensures that all data (e.g., contacts, photos, health metrics) is synced across all devices in the ecosystem. 

5. Software Integration
The ecosystem relies heavily on software and apps designed to improve productivity, health, entertainment, and communication. 
<img width="720" alt="Ecosystem Diagram" src="assets\Files\Diagram\Slide 4_3 - 1.jpg">

**Reflection**

Creating the diagram of personal devices made me realize the importance of sensing technologies and how sensors are becoming more embeded in our daily environments to support new interactions. For example, I looked into the Mites sensor.

<img width="720" alt="sensor" src="assets\Files\layout-2.jpg">

It collects data in the environment such as light, motion, temperature...to infer activities happening in the room.
There are many potential services that comes with this technology, but also concerns regarding data awareness & transparency.

<img width="720" alt="sensor middleware" src="assets\Files\middleware.jpg">



**Speculation**

As the Internet of Things (IoT) continues to expand, IoT sensors are poised to play a transformative role across industries and daily life. Future IoT sensors will become increasingly miniaturized, autonomous, and capable of real-time decision-making through edge computing. These sensors will enable smarter environments. Additionally, advances in AI will allow sensors to analyze complex data locally, providing actionable insights without the need for cloud connectivity, reducing latency and bandwidth usage. This shift could lead to an explosion of interconnected smart devices that make human environments more adaptive, efficient, and responsive.



# Week 3 #
## Week of 09/16/2024
  - Grasshopper Experiments -Part 1
    
    For the next step, I deceded to make a poly-poly pen holder. Here is the working fill in progress: [progress file](assets\RockingPenHolder.gh)

    I found it helpful to draw out a diagram of how I think it should be constructed before I start.
    ![diagram before](image.png)

    As I start actually making the flow, I realized the differences between my mental model of how to construct things and how grasshopper work. 

    Example 1: Constructing an Ellipsoid

    At first, I thought of constructing an ellipsoid from three ellipses,but then I realized that there are no node that can take three curves and turn them into an ellipsoid form.
    <img width="720" alt="ellipsoid before" src="assets\Screenshot 2024-09-14 163605.png">
    
    I then decided to create a sphere first and modify the x,y,z ratio to achieve the same effect.
    <img width="720" alt="ellipsoid after" src="assets\Screenshot 2024-09-14 165138.png">

  - Grasshopper Experiments -Part 2

    To maximize the stability of the pen holder. The top part needs to be as light as possible. That's where lattice will become helpful!

    Here are some cube structures I made:
    [Sturcture 1](assets\lattice\sturcture1.stl), [Sturcture 2](assets\lattice\structure2.stl) , [Sturcture 3](assets\lattice\structure3.stl), [Sturcture 4](assets\lattice\structure4.stl)

    <img width="720" alt="cube strutcure" src="assets\Screenshot 2024-09-16 153904.png">


    I went to the advanced 3D-printing lab to print these cube structures using the Form 3. 


    <img width="200" alt="cube strutcure" src="assets\lattice\7L3A9251.JPG"> <img width="360" alt="cube strutcure" src="image-2.png">



    I ran into Chris Parsell in the lab. I asked him about how some of the 3D print samples on the table were made. I was particularly interested in this Voronoi vase. It seems like a good way to reduce the mass of my Pen holder's top part.

    ![inspo](image-1.png)

    So, I set off creating system to generate the voronoi structure. I talked to Cody about potential ways to do so, and managed to create the lines of the voronoi lattice based on the top part of my pen holder. However, I ran into a problem of uniting individual cells to a single structure. Below are some screenshots of the result.

    <img width="360" alt="test 2" src="assets\lattice\test2.png"> <img width="360" alt="test 3" src="assets\lattice\test3.png">

    Because I was running out of time, I tried to print it despite the segmented breps. I think that the 3D printer has some processing capability to see them as a unity, so the print came out OK.

    <img width="720" alt="test 2" src="assets\photo of holder\7L3A9244.JPG
">

Here is the final Grasshopper File: [Final File](assets\Files\RockingPenHolder_Sep19.gh)


    






    





# Week 2 #
## Week of 09/09/2024

09/09

  - Grasshopper Experiments
  - As a beginner to grasshopper, I first started to explore the files by moving the parameters. Some add-ons or plug-ins are not installed correctly so I cannot display the student and the activity data. Below are  some explorations from adjusting the parameters.
    ![Screenshot 2024-09-09 151131](https://github.com/user-attachments/assets/9e8ad153-ea24-4d1a-b384-4b0fd5590ab6)
    ![Screenshot 2024-09-09 151113](https://github.com/user-attachments/assets/8743e9d8-1d69-4579-9760-2318a2fe56e0)
    ![Screenshot 2024-09-09 151100](https://github.com/user-attachments/assets/15f5b06f-7175-4dd1-8c64-f934a05fa3d9)
  - After the exploration, I made a diagram in figjam:
  - ![diagram](https://github.com/user-attachments/assets/64159e84-cd57-4c38-90d0-b03b7b811e13)

  - During class on Monday, we made this flow in GH that subtract a cylinder from a box.
   <img width="1524" alt="workshop" src="https://github.com/user-attachments/assets/07c00248-f9ec-4ed0-88f2-b43429a62f60">
   
09/12

  - After further exploring the grasshopper file, I used a more visual way of representing the process. Through sketching out how the geometry transforms, I realized that I didn't know how the cut on top of the sphere came from. Then, I discovered that the phone screen offset edge projects itself along the viewing angle with offset to subtract the void from the sphere base.
  ![void Projection](assets/projection.png)
  <img width="400" alt="diagram" src="assets/diagram2.jpg"> <img width="200" alt="vertial phone stand" src="assets/vertialphone.png">

  - I decided that I want to make a phone stand for **video chat**, which means the phone needs to be oriented vertially. After adjusting the phone dimension to an iPhone 14 Plus, it became more difficult to find a design that passes all the test. This is one of the iteration that works.
  ![vertial phone stand 2](assets/iphone14Plus.png)
  This structure looks really chuncky. I want to optimize it's structure.

  - I am curious about how to generate interesting structures with patterns in grasshopper. I found out an online-course about Grasshopper structure by Nolan Kim, a pattern, structural, and computational designer.
    - First, I am introduced to the idea of beam based structure.[more about structure](https://msestudent.com/what-is-the-difference-between-fcc-and-bcc-crystal-structure-properties-interstitial-sites-and-examples/)
    Here are some examples of how it is generated,constructed,and 3d printed.
  ![variations](assets/variationsBeam.png)
  <img width="310" alt="beam based structure" src="assets/beamBasedStructures.png"> <img width="300" alt="3DPrinted" src="assets/exampleof3DPrint.png"> <img width="290" alt="how it generate" src="assets/howItGenerate.png">

# Week 1 #
## Week of 09/05/2024

### Reflections
  - reflections on what you learned and how you learned it
    - This week, I focused on orienting myself in this new environment and setting an optimal workflow. I searched for resources to stay up to date with the emerging technologies. I will curate a list of websites/blogs/plateforms as I go. The hope is to replace 50% of my time used on social media with these material.
        - [Times Magazine](https://time.com/tag/technology/)
        - [ACM Digital Libaray](https://dl.acm.org/)
        - [MIT News](https://news.mit.edu/topic/research)
        - [MIT Media Lab Publication](https://www.media.mit.edu/research/?filter=publications)
  - I tried out the laser cutter and made this keychain
  - <img width="200" alt="laser cutted key chain" src="assets/lasercut.png">
### Speculations
  - AI will increasingly influence every aspect of our life. I recently ran into this [thesis paper from MIT Media Lab](https://www.media.mit.edu/publications/cyborg-psychology/) about “Cyborg Psychology,” an interdisciplinary, human-centered approach to understanding how AI systems influence human psychological processes.
  - ![image](https://github.com/user-attachments/assets/c0887d65-f0ae-43cd-8224-0c3533482763)



---

# Github Background Information & Context
If you’re new to GitHub, you can think of this as a shared file space (like a Google Drive folder, or a like a USB drive that’s hosted online.) 

This is your space to store project files, videos, PDFs, notes, images, etc., and (hopefully, neatly) organize so it's easy for viewers (and you!) to navigate. That said, it’s super easy for you to share any file or folder with us (your TDF instructional team) - just send us the link!  As a start, feel free to simply add images to the `/assets` folder, which is located [here](/assets). 

The specific file that I’m typing into right now is the **README.md** for this repo. 
##### (💡 TIP: The .md indicates that we’re using [Markdown formatting.](https://www.markdownguide.org/cheat-sheet/)) #####
<h6> (💡 TIP 2: GitHub Markdown supports <a href="https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2"> <em>HTML formatting</em> too, including emojis 😄</a>, in case that helps!) </h6>

### :star: Whatever you write in your **README.md** will show up on the “front page” of your GitHub repo. This is where we’ll be looking for your [weekly progress reports](https://github.com/Berkeley-MDes/24f-desinv-202/wiki/3.0-Weekly-Submissions#weekly-progress-report). They might look something like this: ###

# Example Report 1 #
## Week of 09/05/2024

This week, I designed a cool phone stand made of rocks. Check out all my cool sketches and progress photos from this week below, etc., etc....

<img width="200" alt="Cool Phone Stand made of rocks" src="assets/exampleimg.png">

---

It's time to start making this space your own! If you want to save these instructions, make a copy.  Also, feel empowered to delete everything in this README.md and start documenting! 

Excited to work with you,
your TDF teaching team

PS: let us know if you have any questions!!

PPS: 

## Quick Links, compiled here for your convenience: ##

- [TDF Wiki](https://github.com/Berkeley-MDes/24f-desinv-202/wiki) - the ultimate source for truth and information about the course and assignments
- [Google Drive Folder](https://drive.google.com/drive/u/0/folders/1DJ1b6sSDwHXX6NRcQYt10ivyQSgU0ND6) - slides and other resources
- [bCourses](https://bcourses.berkeley.edu/courses/1537533) - where the grading happens
