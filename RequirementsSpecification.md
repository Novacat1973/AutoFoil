# Introduction
Lorem Ipsum

## Document Purpose
The Requirement Specification collects all requirements for the project from a user perspective.  

It lays out functional and non-functional requirements, and may include a set of use cases that describe user interactions that the software must provide.

## Glossary and Definitions
Lorem Ipsum
|Term|Meaning|
|--|--|
|NACA|National Advisory Committee for Aeronautics|

## Project Description
Lorem Ipsum

# Functional Requirements
> **_NOTE:_**  
> The column "MoSCoW" allows mandatory and optional requirements. It is given in the terms of the standard "MoSCoW" method:
>
>  - M = Must Have
>  - S = Should have
>  - C = Could have
>  - W = Won't have (Exclusion, not used in this document)
> 
> Possible Categories are: 
>
>  - General
>  - Stability
>  - Efficiency
>  - Safety / Fail Safe
>  - UI / UX


| Key    | Summary                                        | Description                                                                                                                                                                                                                                                                                                                                                   | Category           | Status | MoSCoW |
|--------|------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|--------|--------|
| req_1  | Speed dependent start                          | The system should start increasing the foil angle above a certain speed. This reduces unnecessary drag at low speeds.                                                                                                                                                                                                                                         | General            | -      | M      |
| req_2  | Limitation of pith angle                       | While lifting on the foils the pitch angle of the boat should not exceed a certain limit to prevent overshootings and an uncomfortable ride.                                                                                                                                                                                                                  | General            | -      | M      |
| req_3  | Adjustable height                              | The flight height needs to be adjustable from the user, so it can be adapted to the current weather conditions.                                                                                                                                                                                                                                               | UI / UX            | -      | S      |
| req_4  | Controlling all foils individually             | All foils of the system on the daggerboards as well as on the rudders need to be controllable individually so that heel and trim can be adjusted from the system.                                                                                                                                                                                             | General            | -      | M      |
| req_5  | Balance of pitch and heel movements            | To provide a smooth foiling experience pitch and heel movements of the boat needs to be balanced so that the platform is on a level position at all time.                                                                                                                                                                                                     | Stability          | -      | M      |
| req_6  | Acceleration-dependent control                 | If the boat experiences rapid angle changes or accelerations, the system needs to be controlled a bit more agressive to prevnet sudden and strong movements.                                                                                                                                                                                                  | Stability          | -      | S      |
| req_7  | Required sensor information                    | The system needs to get information about the current altitude / hight above the water surface, movements arround the six degrees of freedome and the boat speed.                                                                                                                                                                                             | General            | -      | M      |
| req_8  | Freezing the height reference                  | Depending on the used sensor technology, the height reference needs to be freeced at certain pith or heel angles until the boats positioning is in an excepted range again.                                                                                                                                                                                   | Savety / Fail Safe | -      | M      |
| req_9  | Determination of the crew weight               | For further optimizations the system needs to determine / recognize the current crew weight.                                                                                                                                                                                                                                                                  | Efficiency         | -      | C      |
| req_10 | Optimization of longitudinal center of gravity | Since the system will provide a smooth and levelled foiling experience it won't be possible for the crew to know if they are located to far forward or aft. This might lead to an unefficient operation of the foils and too large angles of attack. The system should signal the crew that they have to ideally position themselves further back or forward. | Efficiency         | -      | C      |
| req_11 | Optimization of transversal center of gravity  | As for the optimization of the longitudinal center of gravity the system should also signal the crew that they shoulp position themselves further leewards or windwards to increase or decrease the current righting moment.                                                                                                                                  | Efficiency         | -      | C      |
| req_12 | Switching off individual flaps                 | The system should recognize if a foil is currently lifted up or not. If it is lifted up the flap controll for this individual flap should be switched off to save electic energy and to preserve the mechanical and electrical components.                                                                                                                    | General            | -      | S      |
| req_13 | Safety Mode                                    | The system should recognize sever weather conditions by itself or the user should be possible to go into a safety mode. With the safety mode active the boat won't fully foil anymore to prevent sudden slamming, capzises or pitchpoles.                                                                                                                     | Safety / Fail Safe | -      | S      |
| req_14 | Data logging                                   | The system should be able to logg all sensor data and flap angles for retrospective analysis of the session.                                                                                                                                                                                                                                                  | UI / UX            | -      | C      |
| req_15 | Interface for data download                    | Recorded data of the system must be downloadable. An interface must be provided for this purpose.                                                                                                                                                                                                                                                             | UI / UX            | -      | C      |


# Non-functional requirements

| Key      | Summary                           | Description | Category | Status | MoSCoW |
|----------|-----------------------------------|-------------|----------|--------|--------|
| nf_req_1 | Efficient foil sections           | c           | d        | e      | f      |
| nf_req_2 | Scalable for different boat sizes | c           | d        | e      | f      |
| nf_req_3 | Low costs                         | c           | d        | e      | f      |
| nf_req_4 | Standardized components           | c           | d        | e      | f      |
