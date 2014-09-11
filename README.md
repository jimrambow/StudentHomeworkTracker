Student Homework Tracker

We are going to be creating a project to keep track of your homework submissions. You will have user authentication to control user homework submissions. A user will submit many assignments as well. The format of the data will be based on Iron Yard location. I should be able to make as many TIY locations as I want. Each location will also have an unlimited number of classes. For instance, if we open a back-end class in the future using Clojure, I should be able to add that as a cohort. Each student (during user registration) should be able to select multiple locations/cohorts to assign themselves to.

There will also be an admin user (the instructor/TA!) that is there to grade the homework assignments as complete or incomplete. The instructor should register just like any other user. They will have to select locations/cohorts. The difference is there should be an admin interface. Any pre-existing admin should be able to edit any user and make them an admin.

When an instructor/TA views a cohort, they should be able to see all students and homeworks for the cohorts they are assigned to. When they click into a homework assignment, they should be able to view the comment stream and add whatever they deem necessary. If an additional student views the cohort, they should be able to see the assignments, BUT NOT THE HOMEWORK SUBMISSIONS. https://github.com/ryanb/cancan - That gem may help with that

A instructor/TA/admin user should be able to create homework assignments. The students will have submissions to that specific homework assignment. Each student can only submit ONCE per submission. Students should be able to edit their submissions.

As a student, when submitting homework, I should be able to fill out all necessary information as well as adding any links deemed necessary. I should be able to edit this homework as well if the instructor requests additional information. Once the homework is submitted, only the instructor should be able to change it's workflow state.

When viewing the homework assignment or a submission, there should be a comment stream. The student and instructor should be able to communicate with each other via this comment stream (very similar to GitHub pull requests) on the submission. All of the students for that cohort should be able to ask general questions about the assignment that all other students should be able to see.

When a comment is created, an email needs to be sent to the opposite user. For example, when a student creates a comment, an email message needs to be send to the instructor (if it's on a submission) or all of the other students (if it's on a homework assignment). When an instructor creates a comment, an email needs to be sent to the student (if it's on a submission) or all of the students (if it's on a homework assignment). The email needs to contain the content of the comment as well.

Requirements:

User authentication
Normal User (students)
Admin User (instructors)
Workflow for homework
New
Reviewing
Complete
Incomplete
Data fields for homework
Name
Homework assignments should be able to have many links
For example: I should be able to add a heroku link, a github link, and whatever else I want to add
https://github.com/ryanb/nested_form - This gem will help you guys out here
https://coderwall.com/p/qwx3qa
Description
Comment Stream
100% Styled. This MUST look good! 