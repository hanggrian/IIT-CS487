# [Homework 4](https://github.com/hanggrian/IIT-CS487/blob/assets/assignments/hw4.pdf): Modeling awareness

> You are designing a wearable device which must make the wearer acceptably
  aware of 3 types of "threats":
>
> - An internal health condition
> - An immediate external safety threat
> - Disinformation intended to destabilize society

## Problem 1

> Describe each of your chosen threats and assess its risk to the wearer.

I pick virtual reality (VR) headset as the chosen form of my wearable device
since VR and augmented reality (AR) are gaining ground recently with the public
announcement of *Apple Vision Pro*.

### Subproblem 1A

> An internal health condition.

Having access to the wearer's forehead, we can theoretically measure brain
activity, eye retina, and breathing. The easiest one to implement, I imagine,
would be reading the blood properties of humans using an optical sensor.<sup>[\[1\]]</sup>
The sensor would beam light to the skin tissue on a point-blank range and
calculate the reflection. I believe this is also the same method most
smartwatches use to measure our blood pressure.

### Subproblem 1B

> An immediate external safety threat.

When users are deeply immersed in the VR ecosystem, it is natural to worry about
unintentionally smashing furniture and harming themselves in the process.
Apple's attempt to solve this issue is blending virtual with actual reality,
giving back some control to the wearer. The more conventional methods are to
install a boundary system or video camera monitoring the user's activity.

### Subproblem 1C

> Disinformation intended to destabilize society.

Some VR headsets are designed to be used in conjunction with online services the
manufacturer sells such as *Meta* and its *Horizon Worlds*. As they are
providing users a platform to connect to other participants, moderation is also
needed to filter misinformation, that is, intentionally spreading lies for
personal or political gain. On a lower level, the system could automatically
obfuscate NSFW content.

## Problem 2

> Specify the devices partners and the CCI protocol for each interface.

A common VR setup includes a headset, an input device, and boundary sensors.
Each is a computer on its own and their communication can be categorized as
local CCI. Since the headset requires internet, network devices such as routers
and modems are included in CCI.

There are also external CCI in play, namely the always-running online services,
arguably the main selling point of the headset. When it believes that a user is
in harm's way, it can trigger calls to emergency services like the police and
fire department.

## Problem 3

> Describe a metric or metrics for specifying SA in each case.

Case | Metrics
--- | ---
An internal health condition | Heart rate and blood volume can be measured by using a light absorption sensor.
An immediate external safety threat | Hand gestures, body posture, and movement are tracked by a combination of a camera and other sensors.
Disinformation intended to destabilize society | Whether or not the shared content is factual and contextual.

## Problem 4

> Specify the HCI which will provide acceptable SA of both the wearer and the
  device.

The device should provide real-time alerts regarding the user's well-being in
the form of visuals displayed on the headset, audio by a small built-in speaker,
and haptic feedback like vibration. The wearer would have to dismiss the risk
assessments by a manual input device or voice command.

## Problem 5

> Describe a test strategy to "prove" #4.

- Compare health data &mdash; Periodically check the wearer's heart rate and
  blood level to look for any irregularity. Assert that the data gathered by the
  device match the real-world record.
- Make sudden movement &mdash; See if the VR system picks up dangerous behavior
  and how fast the detection takes.
- Tell a lie &mdash; Determine if user-generated content is misinformed. If
  unable to determine, provide a context of the topics.

## References

1.  [Castaneda, D., Esparza, A., Ghamari, M., Soltanpur, C., & Nazeran, H. (2018). A review on wearable photoplethysmography sensors and their potential future applications in health care. *International journal of biosensors & bioelectronics, 4*(4), 195.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6426305/)

[\[1\]]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6426305/
