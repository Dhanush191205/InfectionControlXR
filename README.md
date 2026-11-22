# InfectionControlXR

What happens after a learner touches a bed rail, a bedside monitor, and an equipment trolley? InfectionControlXR turns those contacts into a visible trail in a Unity hospital room. Learners can replay the scenario, change their actions, and compare the feedback.

![First-person view inside the simulated patient room](Deliverables/build/img/r3_first_person_hands_build.jpg)

[View the illustrated project walkthrough](Deliverables/InfectionControlXR-Showcase.pdf) � [Read the user guide](Assets/Documentation/README.md) � [Explore the C# implementation](Assets/Scripts)

## Try Room 204

1. Install Unity **6000.6.5f1** through Unity Hub and make Git available on your PATH for the Git-based package dependency.
2. Clone the repository, add its root folder in Unity Hub, and let Unity restore the packages and import the assets.
3. Open `Assets/Scenes/MainMenu.unity`, press **Play**, and start the contaminated patient room training.
4. Use **WASD** and the mouse to move and look. Press **E** to touch the bed rail, monitor, and trolley in sequence. Press **F** to reveal the simulated transfer pathway.
5. Press **R** to restart. Try a different sequence with hand hygiene and compare the trace.

## What you can explore

| Scenario | What the learner can investigate |
| --- | --- |
| Patient room | How successive contacts carry simulated contamination between surfaces |
| Five Moments | Which actions the scenario records as hand hygiene opportunities |
| Multi-bed ward | How movement between patient zones changes the contact history |
| Environmental cleaning | How wipe use and cleaning order appear in the session report |
| PPE practice | How the order of donning and doffing affects simulated self-contamination |

The transfer model illustrates how contacts connect. Its values are educational simulation parameters and do not estimate clinical infection risk.

## How it works

Desktop input and OpenXR controller input reach the same interaction and training commands. The simulation tracks contacts and hygiene actions. Trace View exposes the resulting pathway during play, and the session report summarizes decisions for review.

| Project area | Entry point |
| --- | --- |
| Scenes and environments | [Unity scenes](Assets/Scenes) |
| Rules and transfer mechanics | [Contamination model](Assets/Documentation/v2/CTE_Model.md) |
| Automated checks | [EditMode and PlayMode suites](Assets/Tests) |
| PC VR setup and controller bindings | [Quest Link guide](Assets/Documentation/v2/PC_VR_QuestLink_Guide.md) |
| Models, textures, audio and credits | [Third-party notices](THIRD_PARTY_NOTICES.md) |

**Platform status.** Desktop is the quickest way to try the project. The Windows OpenXR path supports Quest Link / Air Link and has been exercised with simulated controllers. Physical headset tracking, comfort, and performance still need validation.
