# 🛡️ Active Directory User Management Automation

A Python and PowerShell-based tool designed to automate everyday Active Directory (AD) tasks such as user creation, password resets, and group membership management. This tool streamlines administrative tasks and improves productivity by automating routine AD operations.

## 🚀 Features

- **👤 User Creation**: Automates the creation of new Active Directory users based on predefined templates or CSV input.
- **🔑 Password Resets**: Simplifies resetting user passwords and enforcing password policies.
- **🗂️ Group Membership Management**: Adds and removes users from AD groups based on input or role changes.
- **📊 User Reports**: Generates reports of user accounts, group memberships, and last login times.
- **🔄 Scheduled Tasks**: Can be automated to run periodically to ensure up-to-date user data.

## 🛠️ Tech Stack

- **🐍 Python**: Core scripting language for LDAP operations.
- **💻 PowerShell**: Handles native Active Directory commands on Windows.
- **🔗 LDAP**: Used for directory access and modifications.
- **📄 CSV Files**: Input format for batch user creation or updates.

## ⚙️ Getting Started

### Prerequisites

- **Windows Server** with Active Directory configured.
- **PowerShell** with necessary AD modules installed.
- Python 3.x installed on the system for additional scripting.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/ad-user-management.git
    cd ad-user-management
    ```

2. Install necessary Python dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Configure your AD environment in the `config.py` file:
    ```python
    AD_DOMAIN = "yourdomain.com"
    AD_ADMIN = "admin_user"
    AD_PASSWORD = "admin_password"
    ```

4. Run the PowerShell script for basic AD tasks:
    ```bash
    ./ad_user_management.ps1
    ```

5. (Optional) For bulk user creation, run the Python script:
    ```bash
    python3 bulk_user_creation.py --csv users.csv
    ```

### Example AD Tasks Automated

- **Create User**: Automatically creates a new AD user with default attributes.
- **Reset Password**: Resets passwords for existing users in bulk.
- **Update Group Membership**: Adds or removes users from security/distribution groups.
- **Generate Reports**: Creates CSV reports of current AD users and groups.

## 📑 Project Structure

```plaintext
ad-user-management/
│
├── ad_user_management.ps1   # PowerShell script for AD tasks
├── bulk_user_creation.py    # Python script for bulk user management
├── config.py                # Configuration for AD connection
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation (this file)
