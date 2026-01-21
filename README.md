# Entra Intune Audit Tool

## Overview
This tool fetches audit data for Entra-only devices in Intune, ensures device compliance states, and reports installed applications using the Microsoft Graph API.

## Setup Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-username>/entra-intune-audit.git
   cd entra-intune-audit
   ```
2. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Obtain API Token**:
   - Go to the Azure Portal.
   - Register a new application and obtain the Client ID and Secret.
   - Ensure you have permissions for Microsoft Graph API to read device data.

4. **Create a configuration file** `config.py`:
   ```python
   API_TOKEN = 'YOUR_API_TOKEN'
   ```
   > Ensure to keep this token secure and do not expose it in public repositories.

## Usage Instructions
- To run the tool, execute:
  ```bash
  python main.py
  ```
- This will check for device compliance and list installed applications.

## Best Practices
- **Secure your API Token**: Do not hardcode sensitive information. Use environment variables or secure vaults.
- **Code Review and Testing**: Always test your code before deploying to ensure it meets compliance requirements.

## License
This project is licensed under the MIT License.
