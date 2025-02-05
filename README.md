# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

Feature 1: As a user,
I should be able to filter events by city
So that I can see a list of events taking place in that city.

Scenario 1: GIVEN user hasn't searched for any city; WHEN the user opens the app; THEN the user should see a list of upcoming events.
Scenario 2: GIVEN the main page is open; WHEN user starts typing in the city textbox; THEN the user should receive a list of cities (suggestions) that match what they've typed.
Scenario 3: GIVEN user was typing "Berlin" in the city textbox and the list of suggested cities is showing; WHEN the user selects a city (e.g.: "Berlin, Germany") from the list; THEN their city should be changed to that city (i.e: "Berlin, Germany") and the user should receive a list of upcoming events in that city.

Feature 2: As a user,
I should be able to show/hide event details
So that I can get more information on a particular event.

Scenario 1: GIVEN user hasn't selected an event to show details on; WHEN the user sees the list of events in their city; THEN the event element should be collapsed by default.
Scenario 2: GIVEN user wants to see details on an event; WHEN the user selects an event; THEN the event element should expand to show details.
Scenario 3: GIVEN user has an event element open; WHEN they want to stop viewing the details of an event; THEN they can collapse the event element.

Feature 3: As a user,
I should be able to change the number of events displayed
So that I can personalize the app to my liking.

Scenario 1: GIVEN user has not specified a number of events; WHEN the user sees the list of events in their city; THEN the default number of events is set to 32.
Scenario 2: GIVEN user wants to set the number of events to something other than the default (32); WHEN they specify the number of events to change the number displayed; THEN the number of displayed events will change to whatever they set it to.

Feature 4: As a user,
I should be able to access the cached information when offline
So that I don't need to remain online in case the event is somewhere where internet isn't available.

Scenario 1: GIVEN user has connected and cached data; WHEN the user does not have internet connection; THEN the user will still be able to see the cached data.
Scenario 2: GIVEN the user has no connection but has cached data; WHEN the user tries to change the search settings (city, number of events, etc.); THEN the user will be shown an error.

Feature 5: As a user,
I should be able to add an app shortcut to my homescreen
So that I can quickly access the app from my device.

Scenario 1: GIVEN user has not installed the meet app already; WHEN the user installs the meet app; THEN the user will have a shortcut to the meet app on their device home screen.

Feature 6: As a user,
I should be able to see charts visualizing event details
So that I can see the number of upcoming events in each city.

Scenario 1: GIVEN the user has not selected a city; WHEN the user sees the list of cities available; THEN the user will also see a chart with the number of upcoming events in each city.
