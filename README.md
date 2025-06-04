

**Overview
**
This article provides guidance on using a custom bash script to back up F5 Distributed Cloud (F5XC) configurations, including:

**Application Namespaces
HTTP and TCP Load Balancers
Origin Pools
Health Checks
Application Firewalls
Service Policies**

The script utilizes the F5XC API for fetching configuration details of various components and organizing them into easily accessible backups.



Before running the script:

Install curl
Ensure curl is installed and available for making API requests.





Install jq
The script uses jq to parse JSON responses from the F5XC API.



Set the Required Variables:
The script requires two variables to be set:

TENANT: Your F5XC tenant name.
API_TOKEN: The token for authenticating requests to the F5XC API.






How to Use
1. Save the Script

Copy the provided script into a file on your system, naming it something like xc-backup.sh.

2. Set Permissions

Run the following command to make the script executable:

chmod +x xc-backup.sh

3. Edit Variables

Before running, set the TENANT and API_TOKEN variables within the script. For example:

API_TOKEN="your_api_token_here"
TENANT="your_tenant_name_here"

4. Run the Script

Run the script and follow the menu prompts:

1

./xc-backup.sh

The script displays a menu: ```
F5 Distributed Cloud

What do you want to backup?

Tenant
Namespace
Load balancer
Quit

#?
