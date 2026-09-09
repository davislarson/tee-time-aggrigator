repo: davislarson/tee-time-aggrigator
branch: main

github pages link: https://davislarson.github.io/tee-time-aggrigator/

1. Questions
   - Need - There are often tens of golf courses within a manageable driving distance from any given location. Each course has its own website and tee sheet, which makes it time consuming to find an open tee time that works for a user. When actually playing is more important then the specific course, the user needs a way to find an open tee time across multiple courses in one place.
   - Persona - A full-time working professional who enjoys golf and plays 2-4 times a month. They have a busy schedule and often have to plan tee times around work and family obligations. 
   - Primary Capability - Find an open tee time across multiple courses in one place. 
   - Fundamental Value - Not spend excessive time and energy searching for a tee time, when only specific times work for the user.



2. Screens

   ## Screen 1 - Parameter Setup
   - State to the user what the application does. Allow the user to manipulate different parameters based on their needs. Parameters include: date, time, number of players, and course location. This page is needed to narrow down the search results and find the best tee time for the user.

   ## Screen 2 - Tee Time Results
   - Display the results of the tee time search based on the parameters set in Screen 1. Organize by course and time, and allow the user to select a tee time to book. This page is needed to allow the user to see all available tee times and select the one that works best for them.

   ## Screen 3 - Booking Confirmation
   - After a user selects their desired tee time, display the details of the booking and allow them to call the pro-shop to confirm the booking, move to the website to book online, or book in-app. This page is needed to ensure the user has all the information they need to complete their booking and confirm their tee time.

3. Design question plan

| Question | Answer |
| --- | --- |
| When was the last time you wanted to book a tee time for a specific day and time but had to look at 4 different websites to find an option that worked? | This happens almost every time I want to book a foursome tee time for my friends and I. I usually go to the closest course first and then check the other courses in the area to see if they have any openings. It can be a time consuming process and I often end up settling for a time that isn't ideal. |
| What would have to be true for you to decide to find a different solution rather than manually looking for tee times across multiple websites? | If there was an easy way to see all available tee times in my area without having to visit many websites. Or if there was a way to move between websites while keeping the same day and time in my search. |
| Who else do you know that deals with this problem? | My friends and family that golf somewhat irregularly. They find that if they are not consistently booking times it becomes more difficult to find a suitable time. |
| I am going to show you this screen for five seconds. What does this product do? | It looks to take all the tee sheets from nearby courses and display them in one place. |

4. First Read

| Question | Answer |
| --- | --- |
| Does the landing screen signal capability + value before reading? | Yes it is quick to state the value, it makes it easy to read the word fast. The Capability requires a little more reading, it is not clear at first glance that it collects tee times from multiple courses. The map is a good indicator that it is looking for multiple course nearby but more investigation is needed.|
| Does every element earn its place on the screen? | I would say yes, everything that is taking space is required to communicate the value and perform the capability. |
| What information and actions belong together, are they using Gestalt grouping?| Sort of, I initially decided to add a map to the right side of the screen to let users know where the system was basing its search, but this is separated from the distance parameter. This base location is part of the parameters and is physically separated from the other parameters. The second page is using common-region boundaries to define what goes together otherwise the courses would be confusing to mentally separate. THe third page has a good common-region boundary to separate the booking actions from the other information on the page.| 
| Do screens 2 and 3 stay on mission, and can you always get home? | Yes, there is a breadcrumb type trail at the top that allows you to navigate between pages seamlessly. The third page somewhat deviates from the mission, it adds more ancillary functionality that is not needed to fulfill the core functionality of booking the tee time. (it allows the user to send reservation details to other people.)|

NOTE: One important change that I made was to add a map to the first screen to show the user where the system is searching for tee times and where the golf courses are in relation to the user's location. Before there was a paragraph stating that there were X number of courses nearby. This might was not helpful to the capability of the system. It lacked a visual representation of where the user was searching for tee times. The map is a better representation of the system's capability to change where they can search.

This is the commit where this happens: https://github.com/davislarson/tee-time-aggrigator/commit/42522e1c24eeadbb6b36ffcbdeb1ae031a0708d8

Here is a screenshot of the first screen with the map added:

![Screenshot of the first screen with the map added](AfterTweak.png)