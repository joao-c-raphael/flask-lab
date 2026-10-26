## Lab Overview: Flask Brute Force Simulation

### Prerequisites & Downloads
- **Python:** Download and install the latest Python release.
- **Visual Studio Code (VS Code):** Install the code editor for script development and execution.

### Environment Setup
- Create a dedicated project folder.
- Initialize and activate a Python virtual environment.
  <img width="595" height="23" alt="image" src="https://github.com/user-attachments/assets/d91ff12c-091a-4384-8555-9bca8f1cb363" />

  <img width="697" height="55" alt="image" src="https://github.com/user-attachments/assets/0e88217a-81a9-4c35-98c9-7d1e9809be25" />

- Install required dependencies (`Flask` and `requests`).

### Flask Application Creation
- Create a new Flask application in VS Code and save it within the `flask-lab` directory.
- placeholder

### Wordlist Creation (Users & Passwords)
- Create a new text file in VS Code containing test passwords (`testpwlist.txt`).
- placeholder
- Repeat the process for the username wordlist (`usernames.txt`).

### Attack Script Development
- placeholder
- placeholder

### Running the Flask Server
- placeholder
- Verify application functionality and endpoint accessibility.
- placeholder

### Executing the Attack Script
- Open a new PowerShell terminal and activate the virtual environment.
- Execute the attack script (`python attack.py`).
- placeholder
- **Results & Observations:**
  - The attack script loaded `testpwlist.txt` and `usernames.txt`.
  - It systematically iterated through the password list against the target usernames until valid credentials were confirmed via the "Welcome" success response.
  - Execution terminated early upon finding a successful match on the first targeted user (`admin`), bypassing subsequent usernames.
