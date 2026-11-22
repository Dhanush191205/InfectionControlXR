# InfectionControlXR

Touch a bed rail, a bedside monitor, and an equipment trolley in Room 204. Trace View reveals how simulated contamination moved through those contacts. Replay the scenario with hand hygiene between interactions, then compare the results.

**[Download the Unity project](https://github.com/Dhanush191205/InfectionControlXR/releases/download/v1.0.0/InfectionControlXR-source.zip)** · **[View the six-page walkthrough](https://github.com/Dhanush191205/InfectionControlXR/releases/download/v1.0.0/InfectionControlXR-Showcase.pdf)**

## Run the project

1. Download **InfectionControlXR-source.zip** using the project link above and extract it.
2. In Unity Hub, add the extracted folder containing `Assets`, `Packages`, and `ProjectSettings`. Open it with Unity **6000.6.5f1** and allow the initial import to finish.
3. Open `Assets/Scenes/MainMenu.unity`, press **Play**, and choose the contaminated patient room.
4. Move with **WASD**, look with the mouse, and interact with **E**. Press **F** to inspect the transfer pathway. Press **R** to restart.

## Training scenarios

| Scenario | What learners practise |
| --- | --- |
| Patient room | Trace successive contacts between surfaces |
| Five Moments | Identify hand hygiene opportunities during care |
| Multi-bed ward | Follow contacts across patient zones |
| Environmental cleaning | Review wipe use and cleaning order |
| Protective equipment | Practise donning and doffing and review simulated self-contact |

## Implementation

Desktop and OpenXR input use shared C# training commands and scoring. The package includes the Unity scenes, C# source, automated tests, user guide, and asset credits. The transfer model uses illustrative values for teaching. Physical Quest testing is pending. 

[View the LinkedIn demonstration](https://www.linkedin.com/feed/update/urn:li:activity:7530269066536787968/)
