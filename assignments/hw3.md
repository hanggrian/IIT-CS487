# [Homework 3](https://github.com/hanggrian/IIT-CS487/blob/assets/assignments/hw3.pdf): Embedded system

> Consider a control system which relies on sensors and systems to automatically
  manage an office building:
>
> - Prevents unauthorized access and allows authorized access.
> - Notifies the fire department if it "thinks" there may be a fire.
> - Notifies the police if it "thinks" there is an intruder.
> - Keeps the temperature "comfortable".

## Problem 1

> Draw a context model capturing the system and its "partners".

![](https://github.com/hanggrian/IIT-CS487/raw/assets/assignments/hw3/context_model.svg)

[View diagram file](https://github.com/hanggrian/IIT-CS487/blob/main/assignments/hw3/context_model.drawio)

## Problem 2

> Create a table identifying:
>
> 1.  Each state the control system can be in.
> 1.  Each possible outward transition – both catalyst and destination.

State | Transition
--- | ---
Waiting | Tap card &rarr; Reading
Reading | Unauthorized &rarr; Warning<br>Authorized &rarr; Enter
Warning | Show help message &rarr; Waiting
Checking | Fire found &rarr; Alerting FD<br>Intruder found &rarr; Alerting PD<br>Nothing &rarr; Keep checking
Alerting FD | Ring alarm &rarr; Call FD
Alerting PD | Lock doors &rarr; Call PD
Measuring | Temperature uncomfortable &rarr; Adjust temperature<br>Comfortable &rarr; Keep measuring
Adjusting | Increase temperature &rarr; Keep measuring<br>Decrease temperature &rarr; Keep measuring

## Problem 3

> Describe a control panel which will support the user interactions noted above.

1. Front gate &mdash; Mechanized gate requiring access card to open. A message
   of reading, success, or error is displayed by a screen attached to the gate.
1. Interactable screen in every room &mdash; In addition to software assessing
   CCTV feeds to find malicious behavior, humans can also report manually with a
   screen that is available everywhere.

## Problem 4

> Develop a set of minimal binary commands to support all necessary signaling
  between the control system and its partners.

Binary | Decimal | Command
---: | :--- | ---
`000` | 0 | Unauthorized acces
`001` | 1 | Authorized access
`010` | 2 | Alert fire department
`011` | 3 | Alert police departmen
`100` | 4 | Increase temperature
`101` | 5 | Decrease temperature

## Problem 5

> Use pseudo-code to describe how your system will detect and handle a failure
  of any of the partners.

```kotlin
fun reading(card: AccessCard) {
  try {
    if (!card.isAuthorized()) {
      alert("Unauthorized.")
      return
    }
    // ...
  } catch (e: TimeoutException) {
    // stop the attempt if too long
    alert("Please try again.")
  }
}

fun checking(camera: CCTV) {
  try {
    assess(camera.result)
    // ...
  } catch (e: ConnectionException) {
    // losing connection is suspicious
    log(e.message)
  }
}

fun measuring(sensor: Thermometer) {
  // sudden difference above 20 degree is suspicious
  if (abs(sensor.value - sensor.lastValue) < 20.0) {
    sensor.value = sensor.lastValue
  }
  // ...
}
```
