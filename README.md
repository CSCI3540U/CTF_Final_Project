# CTF_Final_Project

This project contains the requirements for the end-of-term major project, where students will create capture the flag (CTF) challenges.

Please add the names and GitHub usernames of all group members, as of the time of project submission, to the table below.  If only 3 members, you may delete that row.

| #  | Full Name            | GitHub Username |
| -- | -------------------- | --------------- |
| 1  | first1, last1        | username1       |
| 2  | first2, last2        | username2       |
| 3  | first3, last3        | username3       |
| 4  | first4, last4        | username4       |

## Requirements

### Overview

This project will be completed in a team of 3-4 students.  It has been designed to maximize the team member's ability to work independently.  Teams will need to organize together at the start of the project, when planning their challenges.  Individuals can then work on their challenges.  Individuals can work on their write-up or video walkthroughs for the challenges once the challenges are complete.  Finally, teams will collaborate to plan the presentation.

### CTF Challenges

Each member of the team will create one capture the flag challenge.  The type of challenge is up to the team member.  Examples could include a web application with a XSS vulnerability, an application that had a directory traversal vulnerability, an Android application with some hidden secrets to be reverse engineered, a binary that can be exploited, etc.  You can decide the level of difficulty of the challenge, but the more sophisticated the challenge (i.e. more work involved), the higher likelihood of getting a better score will be.  Any challenge that covers what we did in the lectures, is acceptable as a topic.  However, it is recommended that each challenge goes a bit beyond what we learned (but still relevant within software security).  If you are uncertain if a topic is relevant/appropriate, you are welcome to verify with the instructor.

Each challenge will be in the same repository, but within a directory which will follow the format `challenge_name_difficulty_level`.  For example, a challenge named `Find the Password` which is Medium difficulty, could be in a directory named `find_the_password_medium`.

**Note:  All students in the course must have a unique challenge, and must do the work on their challenge on their own.  It is ok to discuss and plan collaboratively, but the coding should be done by each team member, individually.  For the same reason, using generative AI is also not permitted.**

#### Web-based Challenge

If you choose to create a web application for your challenge, you will need to include everything required in order to run your web application in Docker.  If you are new to Docker, here are some basic instructions on [how to use Docker to deploy your web application](https://www.docker.com/blog/docker-for-web-developers/).  Place all required files to deploy your application within your challenge directory, and include a `HOW_TO_RUN.md` which includes the docker command to execute your web application.  This file should not be big, as only the docker command should be required.

**Note: Definitely, try to clone the repository on a fresh virtual machine, and run it in docker to verify that this deployment will work.**

#### Binary Challenge

If your challenge is based on a compiled binary, simply include the resulting binary, a description of the platform required to execute that binary, and the source code used.  For example, you could use the following format:

`PLATFORM.md` - describe the platform requirements (e.g. Linux, amd64, libraries required)
`/bin` - contains your binary
`/src` - contains the source code
`Makefile` - the makefile to build your code (another build tool is also acceptable, but be sure that it is obvious how to use it)

#### Mobile Challenge

If your challenge is based on a compiled binary, simply include the resulting binary, a description of the platform required to execute that binary, and the source code used.  For example, you could use the following format:

`<your_app_name>.apk` - the final android package file to be deployed on a virtual or real device
`/project` - the Android Studio project, including the original source code

**Note: Be sure to have an appropriate `.gitignore` file to avoid unnecessarily large repositories.**

#### Other Challenges

If your challenge doesn't match any of the examples above, such as a game hacking challenge, be sure to contact the instructor to verify that your challenge will be accepted.  The format of submission may differ, depending on the nature of the challenge.

### Write-Up or Video Walkthrough

Each member of the team will create either a write-up or a video walkthrough, showing how to solve the challenge that was created by one of their teammates.

A write-up is a step-by-step guide that shows how to solve the challenge, often with screenshots of every step along the way.  A video walkthrough is similar, but a screen capture of the process of solving it.  In both cases, it is recommended that you fully solve the challenge before you attempt the write-up.  However, keep notes of what commands you used as you solve the challenge, to make it easier to create the write-up/walkthrough.

**Note:  Team members cannot create a write-up or video walkthrough of their own challenge.  They must solve one of the challenges by the other team member.**

### Presentation

In the final week of classes, each team will choose one of their challenges to highlight and will give a presentation about it.  The presentation will be limited to roughly 8 minutes per group, and will consist of the following:

1. Introduction to the specific vulerability (or vulnerabilities) present in the challenge
2. An overview of how to exploit this vulnerability
3. A quick demonstration of exploitation of the vulnerability
4. A description of how to protect against this vulnerability

**Note: Since all members of the group will be required to participate in this presentation, it makes sense that all of the challenges created by that team are part of the same category.**

## Rubric

The marks for all aspects of this project will be subjective.  This is because this project is serving as our final exam.  As a result, expectations are high.  Careful thought should be put into your challenge to ensure that it is the best representation of the knowledge that you have gained in this course.  The expectation is approximately 30 hours of work for each student.  The challenge that best implements each component, as assessed by the markers, will receive the top grade for that component.  The top mark may not be the same for each marking component.

| Weight      | Component                     |
| ----------- | ----------------------------- |
|  5 marks    | Group presentation            |
| 12 marks    | Challenge                     |
|  8 marks    | Write-up or video walkthrough |

**Note: Git logs and source code will be examined to ensure that this work has been split evenly among the team members.  When the work done is pretty even between the team members, teams will be scored collectively and receive the same grade.  If the work done is substantially different, then team members will be given individual scores that reflect on their own contributions to the project.**

## How to Submit

Accepting this assignment has created a clone of this repository in your own GitHub accounts.  You will be expected to push your code for all of the team's challenges to this repository.  

Students' GitHub usernames do not always match students' real names.  So, in order for the markers to identify the students involved, one of the members of the team must submit the URL of their repository to Canvas, with all of the team members' names at the top.  It does not matter who submits, and you are welcome to do so collectively.
