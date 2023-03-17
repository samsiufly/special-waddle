- ### Avoid Kill Apps
  id:: 64147bf9-5e52-4630-8448-befc5c6fce26
  collapsed:: true
	- [How to Run Linux Commands in the Background](https://www.makeuseof.com/run-linux-commands-in-background/#:~:text=Use%20bg%20to%20Send%20Running%20Commands%20to%20the%20Background&text=You%20can%20easily%20send%20such,typing%20jobs%20in%20the%20terminal.)
	- You can also use the '&' symbol to run a command in the background in Ubuntu. To do this, simply append '&' to the end of the command you want to run:
	- `$ "command" &`
	- This will run the command in the background and immediately return you to the command prompt, allowing you to continue using the terminal for other tasks.
	- To manage background processes, you can use tools such as 'ps', 'kill', and 'jobs'.
- ### Kill Apps
  collapsed:: true
	- To kill a background application in Ubuntu, you can follow these steps:
	- 1. Use the 'ps' command to identify the process ID (PID) of the background application you want to kill. For example:
		- `$ ps aux | grep <application-name>`
		- This command will display a list of running processes that match the specified application name, along with their PIDs.
	- 2. Once you have identified the PID of the application, use the 'kill' command to terminate it. For example:
		- `$ kill <PID>`
		- This will send a signal to the specified process to terminate. If the process does not respond to the signal, you can use the 'kill -9' command to force it to terminate:
		- `$ kill -9 <PID>`
	- Alternatively, you can use the 'pkill' command to kill a process by name, without needing to find its PID first. For example:
		- `$ pkill <application-name>`
		- This will send a signal to all processes that match the specified name to terminate. Note that this can be dangerous if there are multiple processes with the same name, so use this command with caution.
- ### Connecting to a Server via SSH in Terminal
	- ````
	  $ ssh 'user'@'IP-Address'
	  ```
-
- ### Skills
	- Clear Terminal via **Ctrl+L / Ctrl+Shift+K** Shortcut
	  background-color:: yellow