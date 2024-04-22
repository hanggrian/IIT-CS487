# Team Design Report: HCA

## Section 1

In this report, we discuss how we designed our homework calendar application.
First, a context diagram was constructed that depicted how each element in our
system interacted with one another, through authentication, synchronization,
data storage, and so on. Next, a workflow chart was created in order to show how
the application would proceed as the user interacts with it. Workflows for
login, sign up, as well as adding, editing, and deleting assignments were
created. Next, pseudocode was constructed to show a general example of what the
backend interactions would look like. Next, a class diagram was created that
displayed all the necessary classes as well as a UML diagram allocating the
required variables to their respective classes. Lastly, a description of the
non-functional requirements was constructed to explain any outside factors that
were also considered during the design process.

## Section 2

![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/context_model.png)

## Section 3

### State machine workflow

![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow1.png)

### Login sequence workflow

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow2.png"/>

### Sign up workflow

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow3.png"/>

### Add assignment workflow

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow4.png"/>

### Edit assignment workflow

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow5.png"/>

### Delete assignment workflow

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/workflow6.png"/>

## Section 4

```
home_screen():
	display all home screen information
	navigate to next screen based on user click

create_account(args):
	email = args[email]
	password = args[password]
	phone = args[phone]

	save_info(email, password, phone)

login(email, password):
	valid = verify_credentials(email, password)
	if valid:
		login_user
	else:
		exception: invalid

create_assignment(args):
	assignment = new assignment(assignment info)
	store assignment locally

delete_assignment(assignment):
	search for assignment locally
	remove assignment from storage
	exit assignment screen

edit_assignment(assignment):
	search local storage for assignment
	navigate to create assignment screen
	populate create screen with assignment info
```

## Section 5

### Use case diagram

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/use_case.png"/>

### Class diagram

<img width="640" src="https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/data.png"/>

## Section 6

When looking to satisfy non-functional requirements, 5 main points were
considered: Performance, Reliability, Usability, Security, and Maintainability.

### Performance

For performance, it's crucial to ensure efficient data storage. We plan to
implement a database that can handle a large number of homework entries
efficiently. Some options we have considered are SQLite, or alternatively
optimizing data retrieval using appropriate indexing techniques. Provided there
is enough time, employing asynchronous operations, such as background threads or
asynchronous programming techniques, would allow time-consuming tasks like data
synchronization or updates to be performed without affecting the responsiveness
of the user interface.

### Reliability

Reliability is another important aspect to consider. We aim to implement
comprehensive error handling mechanisms to gracefully handle exceptions, network
failures, or unexpected scenarios. By displaying meaningful error messages to
users and providing options for recovery or issue reporting, we would be able to
enhance the reliability of the application.

### Usability

Usability is a key factor in the success of any application. Designing a clean
and user-friendly interface with logical navigation and intuitive controls was
our top priority for providing easy usability. An option discussed was offering
customization options as another way to improve usability. Allowing users to
personalize the application by customizing themes, colors, fonts, and
notifications enhances the user experience, but would also consume time that
could be allocated elsewhere. Additionally, we could consider providing
accessibility features to cater to users with different needs provided there is
extra time.

### Security

Security is crucial to protect user data in the application. Provided the
circumstances of our application development, implementing secure user
authentication mechanisms, such as OAuth or OpenID Connect, to authenticate
users securely would be a possible option.

### Maintainability

Maintainability on an application like this one is a much lesser point to focus
on because of the nature of the situation. The easiest and most streamlined way
to secure maintainability is to document the codebase, including classes,
methods, and important components, to aid future maintenance and
troubleshooting.

## Prototype

Login | Sign up
--- | ---
![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype1.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype2.png)

Calendar view | List view | Class view
--- | --- | ---
![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype3.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype4.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype5.png)

Add assignment | View assignment
--- | ---
![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype6.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype7.png)
