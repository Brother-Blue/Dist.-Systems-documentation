# Group 7

# Table of contents
1. [Purpose](#purpose)
    1. [What](#what)
    2. [Why](#why)
    2. [How](#how)
2. [Requirements (SRS)](#requirements)
3. [Architecture (SAD)](#architecture)
4. [Developers](#developers)

## Purpose <a name="purpose"></a>
### What are you going to make? <a name="what"></a>
We will build a web-application that allows citizens of Gothenburg to book dentist appointments. 
The application will display a map that the user can navigate and find dentist offices.
In the application the user can choose among different dentist offices to book appointments at. 

### Why will you make it? <a name="why"></a>
There is a real demand for this kind of system and as of now there is no available system that 
provides users the opportunity to select from various dentist offices in their area.

### How are you going to make it? <a name="how"></a>
We will build a distributed web-application powered by Node.js and Express using the MQTT-protocol. 

## Requirements (SRS) <a name="requirements"></a>
[Requierments](/Requirements.md)

[User stories](/UserStories.md)

## Architecture (SAD) <a name="architecture"></a>
![Overview](./images/project.png)

First draft of our Architecture for the system:

The system will consist of four different components. 
* Backend that will take care of the database handling. This is where we will store information about users, dentist offices and appointments. Our first draft of the database looks like this:
![ER](./images/er-diagram.png)
* UI is the part that our users get in contact with which will contain a map view of Gothenburg that show available time-slots at different dentists. The UI will let the user book appointments at dentist offices with open time-slots.
* Notifier that will handle email-conformations and other notifications from the system. 
* Logger that handles the logging of previous events to increase our traceability within the system. 

The components mentioned above will mostly communicate through Publish/Subscribe via MQTT. All communications will be handled through a MQTT broker before it is sent to the subscribers. 

As the project moves along this architecture and description will expand and change.

## Developers <a name="developers"></a>

- [Clementine Jensen](https://github.com/clementinejensen)
- [Christian O'Neill](https://github.com/Brother-Blue)
- [Hjalmar Thunberg](https://github.com/Hjalmar-Thunberg)
- [Hugo Hempel](https://github.com/HugoHempel)
- [Linus Ivarsson](https://github.com/linusivarssons)
- [Linus Åberg](https://github.com/LinusAaberg)



