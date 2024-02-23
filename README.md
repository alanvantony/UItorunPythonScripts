# UItorunPythonScripts
Python Django Project to run python scripts from a frontend user Interface 

**This is purely an academic project to learn how Python server side scripts can be run from a User interface in frontend**

SOFTWARE REQUIREMENTS

● Python ● Bootstrap 5 ● Django ● HTML 5 ● CSS3  ● Visual Studio Code - Code Editor 

The front end has a minimal Home page with a button called 'Scripts'. When you click on Scripts , it will redirect to a seperate landing page for Script buttons . In this page,  you will see the buttons for your specific scripts . The footer and header are seperate HTML pages and can be added to other pages as needed . So for testing , I have three buttons in the landing page  'ARP script' - This will run an arp lookup in the backend and return the output to a well formatted HTML page , 'Port Scan' -This is a simple Python script to check for any open ports , 'FindMyIP' - This will find your public IP and return the output to an HTML page . 

You can directly write these Python scripts as functions in views.py and also instead of writing very large functions you can split it up with small ones  . For eg: for an arp lookup,  a simple function called 'get_arp' to do the lookup and then you can call this function from another function 'display_arp'. So whenever 'diplay_arp' is called as an 'action' it will call the get_arp first. The diplay_arp as a seperate function is needed to read the 'ARP' output properly and then render it to an HTML page .  This approach of splitting functions will be useful when you write large functions with lots of read/writes. 

It needs a seperate HTML page for each script to render the script output in a formatted way , also seperate HTML pages are needed to handle errors. The urls.py should also be tweaked accordingly . 


