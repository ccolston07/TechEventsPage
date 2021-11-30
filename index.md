# TechEvents Project Report

Everyday, students at Georgia Tech receive countless emails which can become difficult to manage through simple email inboxes. Many of the emails students receive contain information pertaining to events around campus. However due to the difficulty of managing emails through inboxes, this information is often forgotten, lost, or never even seen by students. A common method across Georgia Tech to create, store, manage, and view events is desperately needed to allieviate the email spam towards students and increase event awareness.

## Software Development Stages

The following sections breakdown the four major stages of our project: planning, requirements, design, and test. Each stage's section overviews our team's thought processes and actions taken.

### Planning Stage

#### Introduction

At the beginning of this project we struggled to come up with an idea for something we could implement that would be both interesting and difficult enough for the assignment. We initialy wanted to created either an iOS exclusive app or some form of video game through Unity. These ideas came from prior experiences some group members had with projects but ultimately we did not have enough commitment into either of these ideas and we did not pursue them. Our final idea we came up with and eventually agreed to work on was the Georgia Tech campus event manager. Each of us agreed that a common frustration we all experienced was in regards to the email spam Tech students recieve and determined that a large majority of these could be eliminated through an email-external event management system. From there we agreed on various features we wanted the app to implement, a rough timeline of when items would need to be completed, our target platform, and our methodological approach to this project. We chose the Waterfall methodology for this project as we felt this best suited both our timescale and the smaller project size for this idea.

#### Project Lifecycle

As mentioned in the introduction, we decided on the waterfall methodology for our approach to this project. This was chosen for a variety of reasons, the first of which being that we did not foresee any changes hapening to the specifications, requirements, or features we had created for this project. This suited the waterfall methodolgy well as this lifecycle does not handle changing requirements well. Addiitonally, we chose waterfall for the sequential nature of the lifecycle. This was important because many features of our app depended on previous features being completed prior and the waterfall methodology requires completing stages before moving onto the next stage. The final reason we chose this lifecycle was due to the time constraints and overall size of this project. We did not have the amount of time needed to run through mutltiple agile iterations like we had done in Project 1, and we limited the number of features we wanted to ensure that we could complete the core aspect of the app on time.

#### Team Communication

Team communication was maintained through two main avenues for this project, GroupMe group chat and weekly BlueJeans meetings. Our group chat was used primarily used to plan our meetings and to keep the team updated on completed tasks or the progress of tasks. As for the meetings, we aimed to have one meeting minimum each week with most weeks having two meetings. The goal behind the meetings was to have weekly progress reports on the project and tasks that were assigned in previous meetings. Additionally, we would lay out new tasks for te week and assign them accordingly to ensure that the project was kept on track. Overall, our team communication was very structured and consistent and this enabled our team to maintain a tight schedule while completing the features we laid out for ourselves.

#### Risk Management

The following table provides a breakdown of risks we foresaw for this project, their severity, likelihood, and potential solution for avoidance.

![Risk Table](/TechEventsPage/Risk_Table.jpeg)

### Requirements Stage

#### Introduction

For our group this stage was fairly short and straightforward, however the importance of this stage cannot be undervalued. During this stage we ensured that our idea and plan that we had created in the previous stage, met all of the requirements laid out to us for the assigment. We felt that the newness to the group of the technologies that we agreed to use added to the difficulty of our idea in regards to the assignment description. Additionally, we felt that the relevancy of solving an issue many students at Tech experience matched well with the assignment description. Overall we felt that after a short analysis of our idea and plan, we could proceed to the design stage of the project as we covered all needed aspects of the assignment.

#### Software Interfaces

1. _Android_
 
   Mobile Operating System based on the Linux Kernel.
   
2. _IOS_

   Mobile Operating System developed by the Apple Inc.
   
3. _expo-cli_

   Command line application that interface between developer and Expo
   
4. _Cloud SDK_
   
   Command line Tool from GCP to communicate between cloud and developer

#### User Interfaces

The user will interact with the system through their mobile device (either iOS or Android device) and the GUI of the project application. The application GUI will offer various methods of interaction including text fields, buttons, and an interactive calendar. These combined aspects will create the interface through which the user can interact directly with the system application.

#### Project Features/Functions

1. Login ability 
  - The user will be able to login using the standard Google account sign-on
2. View Calendar 
  - The user will be able to view a calendar of events that are occurring around campus
3. Create Event
  - Event organizers will be able to add new events with infromation such as start and end times, date, and description

### Design Stage

#### Introduction

During this stage of the assignment we began our implementation of our idea and the plan we had created in previous stages. We had agreed to use the waterfall methodology, and as such, we held 1-2 weekly meetings where we would divide up work to be completed before our next meeting. This allowed us to continually build the app while maintaing our rough schedule we had created in the planning stage and also allowed us to maintain the waterfall approach of completing work before moving onto new items. Alongside this process we also determined that it would be better to divide the frontend and backend work from one another and connect them in the end. This allowed us to maintain our schedule with the time constraints we were experiencing and develop the two sides of the application concurrently. Overall, this ended up working well for our group and allowed us to stay on schedule and complete work that was independent of other areas. The only issue this caused was some difficulties in connecting the frontend and backend back together which would be an aspect to consider in future assignments.

#### System Environment

The system must be a mobile device with a steady internet connection and the ability to run React native compiled code. For Android devices, Expo Go allows easy running of the application from a QR Code generated from our local machines.

#### Architectural (High-level) Design

![Sequence Diagram](/TechEventsPage/Sequence_Diagram.png)

#### Low-level Design

![Component Diagram](/TechEventsPage/Component_Diagram.png)

#### User Interface Design

Click [here](https://www.figma.com/file/1N8p8or2d21CXDu3Tk48UX/EventManager?node-id=0%3A1) for the link to our Figma Prototype we used to plan and design the User Interface.

![Figma Prototype](/TechEventsPage/Figma.png)

### Test Stage

#### Introduction

This final stage of development was done concurrently with the Design stage so that we were able to test alongside the development of new features and ensure that new additions worked entirely as intended. Throughout the development of the application, various testing technologies were used for both the frontend and backend. For the frontend, Expo and ExpoGO were predominantly used to test the user interface. These tools were chosen as they allowed us to test the application, during development, on our own iOS and Android devices. As for the backend, Postman and Jest were the primary technologies used for testing. Postman allowed us to test our API endpoints and to ensure that our calls to our database worked as intended. Jest allowed us to test our JavaScript code to further ensure the functionalities we were creating worked as intended. The concurrent style of testing worked well for our group and this project, allowing us to continually test new features as they were added.

#### Quality Control

We maintained the quality of our testing through a recursive method in which new tests were created with each new feature that was added to the project. These new tests involved writing new coded tests or manually testing the application with the new feature to search for bugs and ensure intended functionality was met. Testing was performed by all group members at each stage to ensure suitable coverage was maintained. Additionally, the criterion we laid out for testing to be deemed completed involved full functionality of the application and all component features as verified by all group members. We believe this worked well with our selected project lifecylce due to the fact that the waterfall methodololgy requires the completion of features before moving onto further stages and features. Ensuring each feature worked completely, and then again as a whole product in the end, allowed us to maintain consistent quaility throughout the development process. However, if any bugs were found through this quality control process, the group communication methods were used such that the chat was notified of an issue and a meeting was scheduled if needed to assign responsibility for resolving the bugs.

#### Test Strategy

The main technologies used for testing involved Jest for testing backend code, Postman for testing API calls and endpoints, and Expo (Expo Go) for manual testing of the user interface and UI functionality. Our main testing strategy for this project was to continually test upon the completion of new features and functionalities. However due to the variety of testing that needed to be done there was no laid out plan for how to test an item. Group communication channels were utilized to disucss testing methods for each addition to the project which enabled every group memeber to test the new code in an appropriate manner. Each group memebr was responsible for testing new additions to the project according to the agreed upon testing method to ensure that the highest amount of bugs were captured through our testing strategy. 

#### Test Cases

The following table outlines our test cases with information regarding action/input, expected and actual output, and any comments we had on the test case.

![Test Cases 1-9](/TechEventsPage/Test_Cases1.png)

![Test Cases 10-17](/TechEventsPage/Test_Cases2.png)

## Technologies

The following lists provide a breakdown of the major technologies used in each area of the project. 

**Frontend:**
  - _React Native_
  - _Expo_
  - _Google Cloud Platform (GCP)_

**Backend:**
  - _Node.js_
  - _Express_
  - _MongoDB_
  - _Postman_
  - _Jest_

## Team Contributions

The following list reviews each team members contribution area for this project in a rough manner. This list does not fully encapsulate project participation but more so a general list of responsibility areas.

1. Frontend Developers:
    - Andy Lee
    - Maksim Tochilkin
2. Backend Developers:
    - Vinnie Davies
    - Maksim Tochilkin
3. Presentation/Project Report
    - Levi Colston

## Project Images

The following images cover the main pages of our application and the functionality of the pages:

![App Sign-on](/TechEventsPage/App-Sign_In.jpeg)

Here you can see the login system for our application which also provides the ability to use the standard Google Sign On system.

![App Creat Event](/TechEventsPage/App-Create_Event.jpeg)

Here you can see the fields we determined were important for creating an event. Each of these fields are saved with the event on our database.

![App Calendar 1](/TechEventsPage/App-Calendar.jpeg)

This image of the calendar demonstrates that selecting a day on the calendar shows an event that occurs on the selected day.

![App Calendar 2](/TechEventsPage/App-Calendar2.jpeg)

This final image of the calendar demonstrates that any given day may have multipple events occuring as well.
