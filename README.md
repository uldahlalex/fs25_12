### Notice: Wednesday is all fullstack and Friday is all AI Apps.

#### Remote repo on Github: `https://github.com/uldahlalex/fs25_12`

## Topics
- New anonymous question approach for presentations
- Activities to wrap up backend portion of the course
    - The role-based feedback app
    - The group-based chat
- Recommendations to using the template_onion repository

<br/>

# Exercises

Today + next Wednesday *(the IoT+Fullstack lesson)* will be **the last potion of the backend** section of the course.  Today's two exercises both wrap up the full scope of the backend portion (+ some client stuff)

They are in varying difficulty, so pick based on your comfort level.

## Exercise A: Live-feedback app *[Easiest]*

*This is the program demonstrated in the beginning of the lesson.*

### Concept
Users anonymously send messages which will be broadcasted to an authenticated user (like students asking anonymous questions in a classroom to a teacher).

Optional features: 
- History (see last X messages) [for teacher]
- Clear recent messages in UI [for teacher]

### Recommended starting point 

I recommend you use the template here: `https://github.com/uldahlalex/template_onion` as a starting point. It follows the same structure as the *fullstack2025* repository, but scaled down.
**If you have your own onion structure with authentication + connection manager, you may also use that as a starting point.**

### Running deployment for the solution: 
`https://yoalex.web.app` (submitting questions view) + `https://yoalex.web.app/alex` (my view)

👉 My solution code for the program is publicly available: `https://github.com/uldahlalex/feedback`


## Exercise B: Group chat app with more complex logic *[Harder]*

### Features
Group chat app features:
- Each chat group has an owner (the "creator of the chat") who can add/remove people
    - There must be role based access control for these actions
- When added to a group chat, all users are notified and the person to enter gets the past 5 messages in the room
- When sending a message to a group, include the message text and sender's ID + email
- Show an indicator of all online people in the system
- Show an indicator of all online people in the same group
- A person can leave the group themselves (without being kicked by admin)
- All actions require JWT authentication (+ role based for admin)

👉 Exercise B (being the harder exercise) starts off without a solution example, but will feature one later.


### Recommended starting point
Just like exercise A, I recommend you use the template here: `https://github.com/uldahlalex/template_onion` as a starting point. It follows the same structure as the *fullstack2025* repository, but scaled down.


<br/>

<br/>


# Resources

### Onion template in minimalist style (just the basics)
Now that you've been sweating with the setup, here's a template with just the basics:

Link: `https://github.com/uldahlalex/template_onion`

(It's **without** the following: Fancy logger, MQTT/IoT stuff, additional wrappers/adapters, event handlers, but still **includes** the REST+Ws Kahoot example and authentication, AppOptions, etc.)