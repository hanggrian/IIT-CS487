# Team Analysis Report: HCA

## Section 1

Our desired app is a calendar to track homework assignments for students. The
application will allow students to input homework assignments assigned to them
divided up by class and due date and allow the student to track their
assignments in one convenient place. We will allow students to look at their
assignments in a list-based format as well as a calendar-based format to allow
for simple tracking of assignments. We will also add a notification system to
notify students at a desired time before the due date to do their homework.
Overall, we wish to create a tracking application that makes it easier for
students to track their homework assignments.

## Section 2

The application is intended for students only and makes no distinction between
student categories. The students can create, track assignments, and be reminded
by notification alerts.

## Section 3

**Functional requirements**:

1. User Registration &mdash; The app must allow students to create user accounts
  using their first and last name, Student ID, student email addresses and
  passwords and phone number.
2. User login &mdash; The app must allow students to login either using their
  email addresses or student ID and passwords.
3. Input Homework Assignments &mdash; The app should provide a form or interface
  for students to input their homework assignments including the name of the
  assignment, the due date, and the class.
4. Class and Due Date Organization &mdash; The app must enable students to
  categorize assignments based on class and specify due dates.
5. Assignment Tracking &mdash; The app must allow students to view and track
  their assignments in one convenient and centralized location. The app should
  display a list of all assignments, including the name of the assignment, the
  due date, and the class.
6. List-Based View &mdash; The app should present assignments in a list format
  for easy reference and tracking. The list should be sorted by due date, with
  the most imminent assignments appearing at the top of the list.
7. Calendar-Based View &mdash; The app should also provide a calendar view to
  allow students to visualize their assignments based on due dates. The calendar
  should display all assignments, with the due dates highlighted.
8. Notification System &mdash; The app must add a notification system to notify
  students at a desired time before assignment due dates.

**Non-Functional requirements**:

1. User-Friendly Interface &mdash; The app must be user-friendly and easy to use
  UI for seamless navigation and interaction. The app should use clear and
  concise language, and it should be easy to find the features that students
  need.
2. Accessibility &mdash; The app must ensure that it is accessible to student
  users with disabilities, adhering to relevant accessibility guidelines. The
  app should provide features such as text-to-speech and zoom, and it should be
  easy to navigate using a keyboard or a screen reader.
3. Performance &mdash; The app must perform efficiently, with quick loading
  times and responsive interactions. The app should not crash or freeze, and it
  should be able to handle many assignments without significant performance
  degradation.
4. Security &mdash; The app must be secure and have appropriate security
  measures to protect student data and prevent unauthorized access. The app
  should require students to create strong passwords.
5. Scalability &mdash; The app should be able to handle a potentially large
  number of student users and assignments without significant performance
  degradation. The app should be able to scale up to handle more users and
  assignments as needed.

**Environmental requirements**:

1. Platform Compatibility &mdash; The app must be able to run with mobile
  Android platform.
2. Network Connectivity &mdash; The app must be able to connect to the internet
  to access and sync student data and send notifications. The app should be able
  to work even if the internet connection is slow or intermittent.

## Section 4

**Test cases**:

1. Adding a Homework Task
    - Description &mdash; This test case verifies if the calendar correctly adds
      a homework task.
    - Steps:
      - Open the homework calendar application.
      - Navigate to the desired date where you want to add a homework task.
      - Click on the "Add Task" button.
      - Enter the task details such as subject, due date, and description.
      - Save the task and close the calendar.
    - Expected Result &mdash; The task should be successfully added to the
      calendar on the specified date.
2. Adding a Homework Task
    - Description &mdash; This test case verifies if the calendar correctly adds
      a homework task.
    - Steps:
      - Open the homework calendar application.
      - Navigate to the desired date where you want to add a homework task.
      - Click on the "Add Task" button.
      - Enter the task details such as subject, due date, and description.
      - Save the task and close the calendar.
    - Expected Result &mdash; The task should be successfully added to the
      calendar on the specified date.
3. Deleting a Homework Task
    - Description &mdash; This test case checks if the calendar allows the
      deletion of a homework task.
    - Steps:
      - Open the homework calendar application.
      - Navigate to the date that contains the task you want to delete.
      - Locate the task and click on it to open the task details.
      - Find and click on the "Delete" button or option.
      - Confirm the deletion when prompted and close the calendar.
    - Expected Result &mdash; The task should be successfully deleted from the
      calendar
4. Logging into the Application
    - Description &mdash; This test case verifies the login functionality of the
    application.
    - Steps:
      - Open the application login page.
      - Enter a valid username and password combination.
      - Click on the "Login" button.
      - Wait for the application to authenticate the credentials.
    - Expected Result &mdash; The application should successfully log in the
      user and redirect them to the main dashboard or home page.
5. Receiving Notifications
    - Description &mdash; This test case checks if the application properly
      delivers notifications to the user.
    - Steps:
      - Log in to the application using valid credentials.
      - Navigate to the user settings or preferences section.
      - Enable or configure the notification settings to receive notifications.
      - Perform an action in the application that triggers a notification, such
        as receiving a new message or completing a task.
      - Wait for the notification to appear on the user interface or in the
        notification center.
    - Expected Result &mdash; The application should successfully deliver the
      notification to the user in a timely manner, either through a pop-up
      message, email, push notification, or any other designated method based on
      the user's settings.
6. Setting Up an Account
    - Description &mdash; This test case verifies the account setup process for new users.
    - Steps:
      - Open the application's registration or account setup page.
      - Fill in the required fields, such as username, email address, and
        password.
      - Provide any additional information or preferences as required.
      - Submit the registration form.
      - Check for any confirmation message or email indicating a successful
        account setup.
    - Expected Result &mdash; The account should be successfully created, and
      the user should receive confirmation of the account setup.
7. Handling Duplicate Account Setup
    - Description &mdash; This test case ensures that the application handles
      duplicate account setup attempts appropriately.
    - Steps:
      - Open the application's registration or account setup page.
      - Fill in the required fields, such as username, email address, and
        password.
      - Provide the same username or email address that is already associated
        with an existing account.
      - Submit the registration form.
      - Check for any error messages or notifications related to duplicate
        account setup.
    - Expected Result &mdash; The application should detect the duplicate
      account setup attempt and display an appropriate error message, indicating
      that the username or email address is already in use.
8. Logging in with an Incorrect Account
    - Description &mdash; This test case verifies the application's behavior
      when attempting to log in  with incorrect credentials.
    - Steps:
      - Open the application login page.
      - Enter an invalid username or email address and password combination.
      - Click on the "Login" button.
      - Wait for the application to authenticate the provided credentials.
    - Expected Result &mdash; The application should display an appropriate
      error message indicating that the login credentials are incorrect or
      invalid. The user should not be granted access to the system.
