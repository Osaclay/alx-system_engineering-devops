Configuration Management

This project highlights the use of Puppet as a configuration management tool. 
It includes writing Puppet manifest files to create a file, install a package, and execute a command.

Tasks 📃

•	0. Create a file

o	0-create_a_file.pp: Creates a file school in the /tmp directory.
	File permissions: 0744.
	File group: www-data.
	File owner: www-data.
	File content: I love Puppet.

•	1. Install a package

o	1-install_a_package.pp: Installs flask from pip3.

•	2. Execute a command

o	2-execute_a_command.pp: Kills the process “killmenow”.
