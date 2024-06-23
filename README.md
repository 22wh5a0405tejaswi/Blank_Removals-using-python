# Blank_Removals-using-python
"Blank removals" typically refers to the process of cleaning up or sanitizing text by removing unnecessary whitespace characters, such as spaces, tabs, and newline characters. 
1. Imports and Functions:

* from tkinter import *: Imports all functions and classes from the Tkinter module for GUI development.
* import filedialog: Import to use the file dialog for opening files.
* import messagebox: Import to display message boxes for error handling.
* print_invert_triangle(filename) Function:
  * Opens the specified file (filename) and reads its contents.
  * Strips leading and trailing whitespace from the text.
  * Splits the text into words.
  * Initializes variables (n, i, j) for managing a loop to process the text.
  * Constructs output by inverting parts of the text in a specified pattern and returns the processed text.
  
2. GUI Setup (button_click() Function and mywindow Setup):

* button_click() Function:
  * Opens a file dialog (filedialog.askopenfilename()) for the user to select a file.
  * If a file is selected (filename is not empty), it calls print_invert_triangle(filename) to process the file content.
  * Creates a new window (Toplevel()) titled "Inverted Triangle Output" to display the processed text using a Text widget (text_widget).
* mywindow (Main Window) Setup:
   * Creates a main window (Tk() instance) titled "New Project".
   * Sets the initial size (geometry) and minimum size (minsize) of the window.
   * Sets up a canvas (Canvas widget) with a gray background (bg="gray16") and specific dimensions (height=1000, width=1000).
   * Attempts to load and display an image (ttt.jpg) as the background using a Label widget (background_label).
   * Error Handling (try and except Block):
     * Catches TclError (Tkinter error) and displays an error message using messagebox.showerror() if the image loading fails.
* Open File Button (Button widget):
    * Creates a button (Button) labeled "Open File".
    * Positions the button at the center (relx=0.5, rely=0.5, anchor=CENTER) of the main window (mywindow).
* Main Loop (mywindow.mainloop()):
   * Enters the main event loop of the Tkinter application, allowing the GUI to handle user interactions and events.
