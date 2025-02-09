# Website_Blocker
The project aimed to create a Python-based Website Blocker tool to restrict access to specific websites to enhance focus because unrestricted internet usage can lead to distractions, security threats, and reduced productivity. 

In this project, Python-based website blocker modifies the system’s hosts file to redirect unwanted websites to 127.0.0.1 (localhost), preventing users from accessing them. The objective of this project is to create a GUI-based website blocker with help of Tkinter library for windows as well as Linux, which will also have an option to unblock those websites.
The Website Blocker works by modifying the system’s hosts file, which acts like an internal address book for the computer. Normally, when a user enters a website URL in the browser, the computer looks up the correct IP address and connects to the website. However, the Python script alters this process by redirecting blocked websites to 127.0.0.1, which is the local machine’s address. Since there is no actual website hosted at 127.0.0.1, the browser is unable to load the blocked site and displays an error message.
To implement this, the script opens the hosts file and checks if the websites that need to be blocked are already listed. If not, it adds them with 127.0.0.1 as their assigned IP address. If a user later decides to unblock a website, the script removes the corresponding entries from the hosts file. Since the hosts file is a system-protected file, modifying it requires administrator or root permissions.
