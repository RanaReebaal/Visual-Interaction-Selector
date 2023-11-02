
# Visual Interaction Selector

This is a simple web application that allows users to select and track interactions on a mock webpage. The application uses HTML, CSS, and JavaScript to implement the functionality.

## Approach

The approach I followed to create this application was:

- Create a mock webpage that contains some interactive elements, such as buttons, links, video, and dropdown menu. Use the `data-track` attribute to assign a label to each element.
- Implement a tool that allows users to enter and exit "selection mode" by pressing the "S" key. In selection mode, hovering over interactive elements should highlight them with a dashed outline. Clicking on an interactive element should mark it as "selected for tracking" with a green border.
- Once an element is marked for tracking, simulate an event being sent to Google Tag Manager (GTM) every time that element is interacted with. For the purpose of this task, mock the GTM endpoint and display a log message in the console for every event sent. The log message should contain the type of element (e.g., "button", "link") and its label or text.
- Display a dashboard on the side that lists all selected elements and the count of interactions for each. Use event listeners to increment the counters and update the dashboard accordingly.

## Challenges

Some of the challenges I faced while creating this application were:

- How to toggle the selection mode using a keyboard shortcut. I solved this by using the `keydown` event and checking if the pressed key was "S". I also used a variable to store the selection mode status and a class to style the body element accordingly.
- How to prevent the default behavior of interactive elements in selection mode. I solved this by using the `preventDefault` method on the click event object.
- How to mock the GTM endpoint and log the event in the console. I solved this by creating a function that takes an element as an argument and extracts its type and label from the `data-track` attribute. I then used the `console.log` method to display the event information.
- How to update the dashboard with the selected elements and the interaction counts. I solved this by using an array to store the selected elements and a function to update the dashboard list. I also used event listeners to increment the counters and call the function.

## How to run and test

To run and test this application, follow these steps:

- Download or clone this repository to your local machine.
- Open the `index.html` file in your browser.
- Press the "S" key to enter selection mode.
- Hover over interactive elements to see them highlighted.
- Click on interactive elements to mark them for tracking. You should see a green border around them.
- Press the "S" key again to exit selection mode.
- Interact with the marked elements. You should see a log message in the console for each event sent to GTM. You should also see a counter on the dashboard that shows how many times each element was interacted with.
- To unselect an element, enter selection mode again and click on it.


## Live Link



## Contact Details

In case you face any issues or errors while running this project feel free to contact me or create an issue for this repository.
