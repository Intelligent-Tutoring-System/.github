<h1>1 - Getting Started</h1>
<h2>1.1 - Project Overview</h2>
The ITS is an auto-grading system aimed at students and lecturers by providing a system that automates the assessment marking process. This would free up lecturers to tackle more important tasks, and allow students a platform to get instant feedback for their assignment submissions.

<h1>2 - Project Structure</h1>

Here we only demonstrate how the complete system works at a high level, due to inherent differences in the subsystems, subdocuments were produced to explain them more cleanly and concisely.

[Frontend README.md](https://github.com/Intelligent-Tutoring-System/ITS-front#readme)

[Backend README.md](https://github.com/Intelligent-Tutoring-System/ITS-services#readme)

[Database README.md](https://github.com/Intelligent-Tutoring-System/ITS-database#readme)

<h2>2.1 - System Architecture</h2>
A high-level architectural diagram of the system is shown below. Sections 2.2, 2.3, and 2.4 will go more in depth about their individual structure and implementation.

![image](https://github.com/Intelligent-Tutoring-System/.github/assets/126434695/196db828-1b75-4b2e-af39-f81db488d4e6)

The front end system consists of web pages and client side code that the end users directly interact with. It is a web application that allows them to do tasks like viewing assignments and submitting programming files to be graded. The database stores all user and application related data such as user profiles, record of units enrolled by the user, and code submissions submitted by a student. The backend system runs the auto grading process to produce the final grade, it also acts as an API service to process requests from the front end application and query the database accordingly.

The two users included in the current system are students and lecturers(or tutors). Lecturers are able to view tasks in the units they teach, and the submissions made by all students on those tasks. Students can also access similar web pages but can only view submissions made by themselves.

<h1>3 - Git Structure</h1>
The ITS git contains three repositories:

- ITS-Database (front end) https://github.com/Intelligent-Tutoring-System/ITS-front/

- ITS-front (back end) https://github.com/Intelligent-Tutoring-System/ITS-services
  
- ITS-services (database) https://github.com/Intelligent-Tutoring-System/ITS-database
  

Each repository works on a system that functions differently and plays a different role on the ITS platform, accordingly, each repository has its own git pull request strategy and CI/CD settings that can be referred to in their own README.md.

<h1>4 - Accessing the Project</h1>
Access to some elements of the software system may require authentication info or whitelisting by the development team.

**Codebases**
To get access to the git repositories, please find contacts near the end of the document.

<h1>5 - Future Plans</h1>
<h2>5.1 - New features </h2>
<h3>5.1.1 - Grades Page</h3>
Currently, the ITS platform does not have a Grades page for the student to view their grades for a unit. Students have to manually click into each assignment, tutorial, or lab to see the grade they obtained. This feature will improve the quality of life of the students as they have a page dedicated to grades for them to view all the grades they obtained. 

<h3>5.1.2 - Task Calendar</h3>
A task calendar allows the students to track their submission deadlines and release dates so that the students can prepare themselves sufficiently for the upcoming coursework and pressure. 

<h3>5.1.3 - Deadline Notifications</h3>
As the ITS platform is meant to be used as a supplementary platform to student learning instead of a platform that students probably use daily such as Monash Moodle, it might be easy for students to forget about submission deadlines on the infrequently used ITS platform. Thus, sending email notifications to students near any task deadline that they have not produced submissions for is a good way to solve this issue. This can be done easily as the system stores the student’s email address and we can use AWS lambda to send these emails as a task deadline approaches.

<h3>5.1.4 - Drag-and-Drop Files Feature</h3>
The current ITS platform only allows the students and lecturers to upload files by browsing through directories and selecting the files from there. A better version of this should be both browsing and a drag-and-drop action for the users to upload their files. 


<h2>5.2 - Future Releases</h2>

|Release No|Timeline|Main Goals to Achieve|
|--|--|--|
|1|March 2024 - November 2024|Fix the issues written in maintenance plan|
|2|March 2024 - May 2024|Implement feature 5.1.1 and feature 5.1.2|
|3|July 2024 - November 2024|Implement feature 5.1.3 and feature 5.1.2|


<h1>6 - Troubleshooting</h1>
<h2>6.1 - Developer Contacts</h2>
To contact the development team, send an email to Jacky Chok Ming Jie (mcho0068@student.monash.edu or jackychok810@gmail.com)


