# To-Do List App

This app is a basic yet functional to-do list application designed to help users manage their tasks efficiently. Here's a detailed overview of its features and functionality:

<h2>User Interface and Design</h2>

<h3>- Clean and Modern UI</h3> 
  
  The app's interface is visually appealing, featuring a minimalist design with a focus on usability. It uses the "Poppins" font, which gives it a contemporary look, and the background is enhanced with a linear gradient for visual interest.
    
<h3>- Task Input Field</h3> 
  
  Users can easily add new tasks using the input field at the top of the app. The placeholder text "Add your text" guides users on what to do.

<h3>- Add Button</h3>
  
  The bright, red "Add" button is prominent, encouraging users to click and add tasks. The button is styled with rounded corners, making it visually distinct and easy to interact with.
  
<h3>- Task List</h3>
  
  The app displays tasks in a clean, vertical list. Each task is accompanied by a checkbox icon that indicates its completion status, and a small "×" icon on the right for easy deletion.

<h2>Core Functionality</h2>

<h3>- Adding Tasks</h3>

  Users can input text into the input box and click the "Add" button to create a new task. The app checks if the input field is empty; if it is, an alert prompts the user to enter some text.
  When a task is added, it's displayed as a list item with an accompanying delete button.

<h3>- Marking Tasks as Completed</h3>

  Clicking on a task toggles its completion status. Completed tasks are visually distinguished by a line-through effect and a color change, giving clear feedback to the user.

<h3>- Deleting Tasks</h3>

  Each task has a delete button (represented by a "×") that allows users to remove tasks. Clicking this button instantly deletes the task from the list.

<h3>- Data Persistence</h3>

  The app uses the browser's localStorage to save tasks. This ensures that tasks persist even after the page is refreshed or the browser is closed. The list of tasks is automatically loaded from localStorage when the app is reopened.

<h2>JavaScript Functions</h2>

<h3>- addTask()</h3>

  This function handles the creation of new tasks. It checks if the input field is empty, creates a new task element if it's not, adds a delete button to it, and appends it to the task list. After a task is added, the input field is cleared, and the current task list is saved to localStorage.

    function addTask() {
      // Function implementation
    }
    
<h3>- saveData()</h3>

  This function saves the current state of the task list to localStorage. It stores the HTML content of the task list under the key "data", allowing for easy retrieval later.

    function saveData() {
      // Function implementation
    }
    
<h3>- showTask()</h3>

  This function retrieves the saved task list from localStorage and displays it when the app is loaded. It ensures that users can continue where they left off, with all their tasks intact.

    function showTask() {
      // Function implementation
    }

<h3>- Event Listener on Task List</h3>

An event listener is attached to the task list container to handle user interactions. It listens for clicks on tasks (<li> elements) to toggle their completion status and on delete buttons (<span> elements) to remove tasks. This approach is efficient because it delegates the event handling to the parent container, rather than attaching individual listeners to each task.

    listContainer.addEventListener("click", function (e) {
      // Function implementation
    }
    
<h2>Conclusion</h2>

This to-do list app is a practical example of a simple yet effective web application. It provides essential task management features, ensuring tasks are easy to add, complete, and delete, with the added benefit of persistent data storage. The app's clean design and straightforward functionality make it a user-friendly tool for managing daily tasks.
