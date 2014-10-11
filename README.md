Detailed design and architecture for tracking system
=====================================================
Users: 

There are two kinds of users: A collector, who goes on reports data, and a community moderator, who reviews both individual instances and aggregate reports of activities.

User Tasks: 

A collector can view his or her history of a gps tracked run or ride and upload an associated video clip.
A collector can review the issues that will be reported to a community moderator.
A collector can track and see the status of particular issues.  They can see other reports associated with the same issue.
A collector can get badges and points for issues that have been successfully verified by a community moderator.
A community moderator has a queue of reported issues to review.
A community moderator can reject or verify a reported issue and state a reason.
A community moderator can see an aggregate view of issues that is overlayed on a street map.
A community moderator can elevate an issue to a major concern, which will be brought up at a community meeting.
Any view can be seen on a web device or mobile device.

System Tasks:

The computer vision component supports three types of activities: red light running, debris in bike lanes, and insufficient lane width.
A task that calls the computer vision component and extracts the video frames, time position, suspected type of activity, and set of geometric boundaries and overlays provided by the computer vision component.
A task is needed to calibrate and associate a video frame with a gps position.
A task is needed to distribute frames of videos to different processing nodes that run the computer vision analysis.
A task that determines which community moderator is responsible for a given geographic area.
A task that randomly samples reported issues and adds it to a community moderators queue.
A task that automatically relates two issues if they occur at the same location and report the same type of activity. 


Requirements:

Architecture diagram and description: Describe what architectural pattern(s) you are using and why (at least 300 words).  Should provide a very high level overview of the system while being comprehensive.  Note if you are using a specialized version of an architecture.

Technology Stack.  Research a set of technologies that will fulfil the role of each major architectural component of the system.  Provide a “technology infographic”, describing the selected technologies.

The architecture and technology stack needs to address the following aspects:

Storage
Object-relational mapping (connecting storage to back-end).
3rd party services (map, gps tracking)
Back-end services for front-end
Back-end services for computationally demanding tasks
Distributed computing
Load balancing and monitoring
Mobile client interface technologies
Web client interface technologies

Wireframe model.  Provide an annotated wireframe model of the aggregate report that the community moderator would view.

Class model. In one diagram, provide a detailed class model for the set of classes that would be needed to implement 2 system tasks and 2 user tasks of your choice.  Please provide attributes (no types or visibility), operations (no signatures), and relationships.

2 design patterns: In one diagram, provide a class diagram that implements those patterns.  Provide a brief description describing why you selected those patterns and what problem they help solve (at least 50 words).

Sequence diagram.  Pick one of the user tasks.  Provide a sequence diagram that models the interaction between components of your system to accomplish that task.  Place a text field in the diagram to indicate which task you are modeling.
