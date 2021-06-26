# Application State with Redux

## What are the advantages of storing tokens in “Cookies” vs “Local Storage”
- Cookies are read server-side, and local storage is read client-side, so if the server needs the data, then it is better to use cookies.

##  Explain 3rd party cookies.
- Third-party cookies are cookies that are set by a website other than the one you are currently on. 

## How do pixel tags work?
- Pixel tags are typically single pixel, transparent GIF images that are added to a web page. Even though the pixel tag is virtually invisible, it is still served just like any other image you may see online.

# Term

|    |  |
| ----------- | ----------- |
| cookies      |  They are pieces of code that web servers use to put information on a user’s browser, and then retrieve that information at a later time for various uses.     |
| authorization      |  Authorized the user to go to different areas based on what they are allowed to see and do(allowing a user to access or to do something).     |
| access control      |  This restricts access to different areas of a network based on a person's role in an organization.    |
| conditional rendering      | The ability to render different user interface (UI) markup if a condition is true or false.    |


# Redux

- is an open-source JavaScript library for managing application state. It is most commonly used with libraries such as React or Angular for building user interfaces. Similar to (and inspired by) Facebook’s Flux architecture .

- Redux is a predictable state container for JavaScript apps. As the application grows, it becomes difficult to keep it organized and maintain data flow. Redux solves this problem by managing application’s state with a single global object called Store.

### Technical benefits of using Redux
- Predictable states. The state is always predictable in Redux. 
- Easy in maintenance. 
- Debugging is easy. 
- Testing code is simple. 
- Server rendering. 
- Vast developer tools available. 
- Great supportive community. 
- Reusable Code.

### Redux is more useful when:

- You have large amounts of application state that are needed in many places in the app
- The app state is updated frequently over time
- The logic to update that state may be complex
- The app has a medium or large-sized codebase, and might be worked on by many people

