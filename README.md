**This project is primarily intended for academic purposes, aiming to explore the execution of Python server-side scripts via a frontend user interface.**

SOFTWARE REQUIREMENTS

● Python
● Bootstrap 5
● Django
● HTML 5
● CSS3
● Visual Studio Code - Code Editor

The frontend comprises a minimalist Home page featuring a button labeled 'Scripts'. Upon clicking on 'Scripts', users are redirected to a dedicated landing page for script execution. Here, specific script buttons are displayed. The header and footer are separate HTML pages and can be incorporated into other pages as required. For the purpose of testing, three buttons are provided on the landing page:

.'ARP script': This button executes an ARP lookup in the backend and presents the output in a well-formatted HTML page.

.'Port Scan': Executes a simple Python script to check for open ports.

.'FindMyIP': Identifies the user's public IP and displays the output on an HTML page.
The Python scripts can be implemented directly as functions in views.py. To enhance readability and maintainability, it is recommended to break down large functions into smaller ones. For instance, for an ARP lookup, a function named 'get_arp' can handle the lookup, which can then be called from another function, 'display_arp'. Thus, whenever 'display_arp' is invoked as an action, it initiates the 'get_arp' function first. Utilizing separate functions aids in effectively managing functions with extensive read/write operations.

Each script requires a separate HTML page to present the output in a formatted manner, and dedicated HTML pages are essential for error handling. The urls.py file should be adjusted accordingly to accommodate these requirements.




