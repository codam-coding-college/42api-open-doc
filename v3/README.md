# Intra V3 API
The Intra V3 API is seperated into several sections, each with its own documentation. Below is a summary of the available APIs and their main sources of documentation.


---

## Paced System
Main source of documentation: https://pace-system.42.fr/api/v1/docs
The Paced System API provides information about the paced system, which is a system that allows students to progress through their curriculum at their own pace, setting their own milestones.

### Users
Get information on specific users.

TODO: list endpoints

### Milestones
Retrieve all or individual milestones.

#### /milestones/{milestone_id}
Retrieve a specific milestone by its ID.

#### /milestones
Retrieve all milestones.

### Pace Matrix
TODO: list endpoints

### Paces
TODO: list endpoints

### Campus
Get information about a campus.

TODO: list endpoints


---

## Freezes
Main source of documentation: https://freeze.42.fr/api/v2/docs.
The Freezes API provides information about freezes and user deadlines in the Common Core.

### Me
Get information about the current user.

TODO: list endpoints

### Campus
Get information about a campus.

TODO: list endpoints

### Freeze Logs
TODO: list endpoints

### Users
Get information about specific users.

TODO: list endpoints

### Freezes
Get information about freezes.

TODO: list endpoints


---

## Chronos
Main source of documentation: https://chronos.42.fr/api/v1/docs#/

### Attendance

#### Attendances
Get the raw attendance data of a user. This lists each attendance event separately, including the start and end time of each event.

#### Base Attendance
Get the attendance data of a user, aggregated by date. Choose the source to get the attendance data from, such as "location" or "vsa".

#### Presence Attendance
Check on which dates a user was present at a campus.


### Campuses
Get an overview of campuses and their available attendance sources.

Sources normally include locations, which are copied over from the Intra V2 API and contain the time users spent behind computers at a campus.

Some campuses might have additional sources. For example, Codam has a source called "VSA" that contains the time users spent in the building.
