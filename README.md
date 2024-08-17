# To-Do-List-App

This app is a basic yet functional to-do list application designed to help users manage their tasks efficiently. Here's a detailed overview of its features and functionality:

1. User Interface and Design

  Clean and Modern UI 
  
  The app's interface is visually appealing, featuring a minimalist design with a focus on usability. It uses the "Poppins" font, which gives it a contemporary look, and the background is enhanced with a linear gradient for visual interest.
    
  Task Input Field 
  
  Users can easily add new tasks using the input field at the top of the app. The placeholder text "Add your text" guides users on what to do.

  Add Button
  
  The bright, red "Add" button is prominent, encouraging users to click and add tasks. The button is styled with rounded corners, making it visually distinct and easy to interact with.
  
  Task List
  
  The app displays tasks in a clean, vertical list. Each task is accompanied by a checkbox icon that indicates its completion status, and a small "×" icon on the right for easy deletion.

2. Core Functionality

  Adding Tasks

  Users can input text into the input box and click the "Add" button to create a new task. The app checks if the input field is empty; if it is, an alert prompts the user to enter some text.
    When a task is added, it's displayed as a list item with an accompanying delete button.

  Marking Tasks as Completed

  Clicking on a task toggles its completion status. Completed tasks are visually distinguished by a line-through effect and a color change, giving clear feedback to the user.

  Deleting Tasks

  Each task has a delete button (represented by a "×") that allows users to remove tasks. Clicking this button instantly deletes the task from the list.

  Data Persistence

  The app uses the browser's localStorage to save tasks. This ensures that tasks persist even after the page is refreshed or the browser is closed. The list of tasks is automatically loaded from localStorage when the app is reopened.

3. JavaScript Functions

  addTask()

    This function handles the creation of new tasks. It checks if the input field is empty, creates a new task element if it's not, adds a delete button to it, and appends it to the task list. After a task is added, the input field is cleared, and the current task list is saved to localStorage.
    
  saveData()

    This function saves the current state of the task list to localStorage. It stores the HTML content of the task list under the key "data", allowing for easy retrieval later.

  showTask()

    This function retrieves the saved task list from localStorage and displays it when the app is loaded. It ensures that users can continue where they left off, with all their tasks intact.

  Event Listener on Task List

    An event listener is attached to the task list container to handle user interactions. It listens for clicks on tasks (<li> elements) to toggle their completion status and on delete buttons (<span> elements) to remove tasks. This approach is efficient because it delegates the event handling to the parent container, rather than attaching individual listeners to each task.
    
Conclusion
This to-do list app is a practical example of a simple yet effective web application. It provides essential task management features, ensuring tasks are easy to add, complete, and delete, with the added benefit of persistent data storage. The app's clean design and straightforward functionality make it a user-friendly tool for managing daily tasks.
