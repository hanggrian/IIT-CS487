# Team Design Report: HCA

## Section 1

Lorem ipsum.

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

Lorem ipsum.

## Prototype

| Login | Sign up |
| --- | --- |
| ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype1.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype2.png) |

| Calendar view | List view | Class view |
| --- | --- | --- |
| ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype3.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype4.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype5.png) |

| Add assignment | View assignment |
| --- | --- |
| ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype6.png) | ![](https://github.com/hendraanggrian/IIT-CS487/raw/assets/hca/prototype7.png) |
