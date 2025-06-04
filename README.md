Bash script to backup F5 Distributed Cloud configuration
Overview
A bash script for backing up the following F5 Distributed Cloud objects:

Application Namespaces
HTTP Load Balancers
TCP Load Balances
Origin Pools
Health checks
Application Firewalls
Service Policies
Requirements
curl - used to fetch object configurations via the F5 Distributed Cloud API
jq - used to format and process responses
Set TENANT and API_TOKEN variables
How to Use
Run the script and select the type of object to backup:

$./xc-backup.sh

---------------------------------
F5 Distributed Cloud
---------------------------------

What do you want to backup?

1) Tenant
2) Namespace
3) Load balancer
4) Quit
#?
