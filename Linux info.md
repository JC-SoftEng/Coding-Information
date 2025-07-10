# How to transfer files from Windows to Linux
# Using SCP (Secure Copy Protocol)
# 1. Open a terminal on your Linux machine.
# 2. Use the following command to copy a file from Windows to Linux:
#    scp /path/to/local/file username@linux_host:/path/to/remote/directory
#    Replace `/path/to/local/file` with the path to the file on your Windows machine,
#    `username` with your Linux username, `linux_host` with the IP address or hostname of your Linux machine,
#    and `/path/to/remote/directory` with the directory on your Linux machine where you want to copy the file.

# How to create a venv in Linux
# 1. Open a terminal.
# 2. Install the `python3-venv` package if it's not already installed:
#    sudo apt install python3-venv
# 3. Navigate to the directory where you want to create the virtual environment.
# 4. Run the following command to create a virtual environment:
#    python3 -m venv myenv
#    Replace `myenv` with the name you want to give to your virtual environment.
# 5. To activate the virtual environment, run:
#    source myenv/bin/activate

# How to find the process ID (PID) of a running process in Linux
# 1. Open a terminal.
# 2. Use the `ps` command to list running processes:
#    ps aux
# 3. Find the process you are interested in and note its PID, which is the number in the second column.
# 4. Alternatively, you can use the `pgrep` command to find the PID of a specific process:
#    pgrep process_name
#    Replace `process_name` with the name of the process you are looking for.