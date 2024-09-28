 
#  Responsive Navbar
Responsive NavBar with dark/light effect

##  Branch 'dev1'

Here we have structured the Navbar skeleton 
![screenshot](pics/screenshot1.png)
***

##  Branches 'dev2' and 'dev3'

These branches contain the style and script for the Navbar and toggle events respectively.
***

## Branch 'joint'

Here we have combined the Navbar skeleton, style and script to create a fully functional Navbar
![screenshot](pics/screenshot2.png)
![screenshot](pics/screenshot3.png)
***

## Branch  'QA'  and 'Main'

Here we have added the testing and deployment scripts respectively.
We also slightly modified the  base color for the dark effect

![screenshot](pics/screenshot4.png)
![screenshot](pics/screenshot5.png)
***

#  Code analysis
 
##  HTML File

We defined a navigation bar with a search box that can be toggled on and off using the provided icons. The search box we included contains an input field and a search icon.
Lastly we linked our base code to the script file, which is resonsible for handling the search functionality, such as toggling the search box and processing search queries.
***

## css file
1- We defined global variables for consistent design elements throughout the stylesheet

2- Then the basic layout and appearance of the body element, including its height and background was set.

3- We continue with the dark mode effects, defining the set of styles that can be applied to the body element to switch to a dark mode theme, overriding the basic body styles.

4- Lastly we styled the navigation bar, including its position, size, and background color, to create a fixed navigation bar at the top of the page.
***

## script file
This JS code is used to toggle between dark and ligth modes on a web page. It also persist the user's preferred mode even after the page refresh or file reopen using local storage.

- **Variable declaration**: We start by declaring several varaiables using **'const'** and **'let'** keywords. These variables are used to store references to HTML elements as follows: **'body'**, **'nav'**, **'modeToggle'**, **'searchToggle'**, **'sidebbarOpen'**, **'sidebarClose'** and **'getMode'**

- **Inittial mode setup**: The code checks if there is a store mode in the local storage using **'localStorage.getItem("mode")'**. If a mode is found and it's equal to **'dark-mode'**, the code adds the **'dark'** class to the **'<body>'** element  using **'body.classList.add("dark")'**. This set the initial mode of the page.

- **Event Listener to Mode Toggle**: This code adds an event listener to the **'modeToggle'** element to listen for clicks. When the element is clicked, the following actions are performed:

1- The **'active'** class is toggled on the **'modeToggle'** element using **'modeToggle.classList.toggle("active")'**.

2- The **'dark'** class is toggled on the **'<body>'** element using **'body.classList.toggle("dark")'**. This toggles the dark mode on or off.

3- The code also checks if the **'<body>'** element has the dark class using **'body.classList.contains("dark")'**. If it doesn't, it sets the mode to **'light-mode'** in local storage using **'localStorage.setItem("mode", "light-mode)'**. If it does, it sets the mode to **'dark.-mode'** in local storage using **'localStorage.setItem("mode, "dark-mode")'**. This ensures that the user's preferred mode is persisted even after page refresh or file reopen.

***

![reading...](https://media.giphy.com/media/Tf3mp01bfrrUc/giphy.gif?cid=ecf05e47wajghtrc5targr7mju7coe0avdyurnehrr1krgdt&ep=v1_gifs_search&rid=giphy.gif&ct=g "...How could I ever do so unless someone guide me?")

***
