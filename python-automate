import os
import getpass

# Define the users and groups
users = {
    "Andrew": "System Administrator",
    "Julius": "Legal",
    "Chizi": "Human Resource Manager",
    "Jeniffer": "Sales Manager",
    "Adeola": "Business Strategist",
    "Bach": "CEO",
    "Gozie": "IT intern",
    "Ogochukwu": "Finance Manager"
    
}

# Define the company directories
directories = [
    "Finance",
    "Budgets",
    "Contract Documents",
    "Business Projections",
    "Business Models",
    "Employee Data",
    "Company Vision and Mission Statement",
    "Server Configuration Script"
]

# Create the users and groups
for user, group in users.items():
    os.system(f"useradd -m {user} -g {group}")

# Create the company directories
for directory in directories:
    os.makedirs(directory, exist_ok=True)

# Take user input to create a file
file_name = input("Enter the name of the file: ")
directory = input("Enter the directory to create the file: ")

if directory in directories:
    with open(os.path.join(directory, file_name), "w") as f:
        f.write("")  # Create an empty file
    print(f"File {file_name} created in directory {directory}")
else:
  print("Invalid directory. File not created.")
