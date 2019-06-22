# Maintenance user
Create a maintenance user with root previlidges

1. Use the adduser command to add a new user to your system: 

`$ sudo adduser maint`

2. Use the passwd command to update the new user's password:

`$ sudo passwd maint`

3. Use the usermod command to add the user to the wheel group (By default, on CentOS, members of the wheel group have sudo privileges) 

`$ sudo usermod -aG wheel maint`

4. Test new user:
login as maint
test a sudo command and verify it's executing correctly ex: 
$ sudo nmtui
