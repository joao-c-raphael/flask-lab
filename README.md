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
  <img width="800" height="780" alt="image" src="https://github.com/user-attachments/assets/c02269c5-cedd-4d84-a2a2-2eab8adcccd9" />

### Wordlist Creation (Users & Passwords)
- Create a new text file in VS Code containing test passwords (`testpwlist.txt`).

  <img width="385" height="186" alt="image" src="https://github.com/user-attachments/assets/ae973650-ec34-4e17-a1d1-2a89973f2c16" />

- Repeat the process for the username wordlist (`usernames.txt`).

### Attack Script Development
  <img width="735" height="1060" alt="image" src="https://github.com/user-attachments/assets/a094f0e0-28eb-4b69-86fe-65091aef963a" />

  <img width="836" height="505" alt="image" src="https://github.com/user-attachments/assets/80fe821a-ae02-43c5-bcbd-17e2cdd97888" />


### Running the Flask Server
  <img width="1427" height="135" alt="image" src="https://github.com/user-attachments/assets/69ac5dcf-17dc-47f6-bd3f-6d20d9aaf799" />

- Verify application functionality and endpoint accessibility.

  <img width="445" height="92" alt="image" src="https://github.com/user-attachments/assets/98109b7c-ed1e-4369-9a46-3bea05a7fca3" />


### Executing the Attack Script
- Open a new PowerShell terminal and activate the virtual environment.
- Execute the attack script (`python attack.py`).

  <img width="645" height="117" alt="image" src="https://github.com/user-attachments/assets/d42a7091-0fcd-4386-9965-0f5bc0b66598" />

- **Results & Observations:**
  - The attack script loaded `testpwlist.txt` and `usernames.txt`.
  - It systematically iterated through the password list against the target usernames until valid credentials were confirmed via the "Welcome" success response.
  - Execution terminated early upon finding a successful match on the first targeted user (`admin`), bypassing subsequent usernames.
