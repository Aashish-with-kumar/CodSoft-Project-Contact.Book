#  Internship Provider CodSoft- Python Programming Project


# Contact Book Application
This Python-based Contact Book Application allows users to manage contacts efficiently. The program stores contact details such as names, phone numbers, and email addresses in a JSON file. It provides functionality to add, view, delete, and search for contacts, with validation for phone numbers.


---

# Features

1. Add Contact:

Add a new contact with a name, phone number, and email address.

Validates phone number length (maximum 10 digits) and ensures it contains only numeric characters.



2. View Contacts:

Displays a list of all saved contacts with their name, phone number, and email.



3. Delete Contact:

Allows users to delete a contact by name.



4. Search Contact:

Search for a specific contact by name and view their details.



5. Data Persistence:

Contact details are stored in a JSON file (contacts.json) for persistent storage.



6. Exit:

Save all changes to the JSON file and exit the application.





---

# How to Use

Step 1: Clone or Download the Project

1. Clone the repository or download the ZIP file to your local machine.



Step 2: Run the Application

Open the terminal or command prompt.

Navigate to the directory where the script is located.

Run the following command:

python <filename>.py


Step 3: Interact with the Application

Choose from the following options displayed in the menu:

 # Contact Book
1. Add Contact
2. View Contacts
3. Delete Contact
4. Search Contact
5. Exit



---

# Code Explanation

1. Data Storage

Contacts are stored in a JSON file named contacts.json.

This ensures that the contact list persists between application runs.


2. Phone Number Validation

Ensures phone numbers are numeric and do not exceed 10 digits:

if len(phone) > 10:
    print("Phone number should not exceed 10 digits.")
if not re.match(r'^\d+$', phone):
    print("Phone number should contain only digits.")


3. Functionalities

a. Add Contact

Prompts the user for contact details (name, phone number, and email).

Validates the phone number before saving.


b. View Contacts

Displays all saved contacts in a readable format.


c. Delete Contact

Deletes a contact by name, if it exists.


d. Search Contact

Allows searching for a contact by name and displays their details.


e. Exit

Saves all changes to contacts.json before exiting.



---

# Example Usage

Adding a Contact

Enter contact name: John Doe
Enter contact phone number: 1234567890
Enter contact email: john.doe@example.com
Contact 'John Doe' added.

Viewing Contacts

Name: John Doe
Phone: 1234567890
Email: john.doe@example.com

Deleting a Contact

Enter contact name to delete: John Doe
Contact 'John Doe' deleted.

Searching for a Contact

Enter contact name to search: John Doe
Name: John Doe
Phone: 1234567890
Email: john.doe@example.com

Exiting

Contacts saved. Exiting...


---

# Dependencies

Python 3.x

No external libraries required; uses built-in Python modules like os, json, and re.



---

# Improvements

Add support for multiple phone numbers or emails for a single contact.

Enhance the user interface using a graphical library like tkinter or PyQt.

Encrypt the JSON file for better security of contact information.



---

# Key Learnings

Data persistence using JSON files.

Input validation using the re module.

Modular programming with reusable functions.



---

This project is ideal for anyone starting with Python and looking to build a functional and practical application.
