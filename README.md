# Digital Clock in Python
This project is a Digital Clock built using Python and the Tkinter library. The clock displays the current time and updates in real-time. The user interface (UI) is simple and uses the Label widget to show the time, updating every second.

Features:
Displays the current time in a 12-hour format (HH:MM:SS AM/PM).

Real-time updating every second.

Simple, clean, and customizable user interface (UI) using Tkinter.

Requirements
To run this project, you need to have the following installed on your system:

Python 3.x

Tkinter (usually bundled with Python by default)

If Tkinter is not installed, you can install it using the following:

bash
Copy
pip install tk
Installation
Clone this repository to your local machine:

bash
Copy
git clone https://github.com/your-username/digital-clock-python.git
Navigate to the project directory:

bash
Copy
cd digital-clock-python
Run the Python script:

bash
Copy
python digital_clock.py
This will open a window with the digital clock showing the current time.

Code Explanation
The code defines a simple Tkinter application with the following components:

Window setup:

my_w = tk.Tk() initializes the Tkinter window.

my_w.geometry("405x170") sets the window size to 405x170 pixels.

Time Update:

my_time() is a function that gets the current time using Python’s strftime() method and formats it in the pattern of HH:MM:SS AM/PM.

The time is displayed using the Label widget (l1) and updates every second using l1.after(1000, my_time).

Font and UI:

The font for the label is set using the my_font variable, which defines the font as 'times', with a size of 52 and bold style.

The background color of the label is set to pink using bg='pink'.

The label is positioned within the window using the grid() method with padding.

Main Loop:

my_w.mainloop() starts the Tkinter event loop, keeping the window active and responsive.

Screenshots

Customization
You can easily customize the clock by changing the following:

Font: Modify the my_font variable to use a different font, size, or style.

Background color: Change the bg parameter in the Label widget to any color of your choice.

Time format: Modify the format string inside strftime() to change the time format (e.g., 24-hour format or different date/time representation).


Acknowledgments
Tkinter for creating the graphical user interface.

Python for providing an easy-to-use programming environment for building the clock.
