````markdown
# How to Transfer Files from Windows to Linux

## Using SCP (Secure Copy Protocol)

1. Open a terminal on your **Linux** machine.
2. Copy a file from Windows to Linux:
    ```bash
    scp /path/to/local/file username@linux_host:/path/to/remote/directory
    ```
````

-   `/path/to/local/file` – path to the file on Windows
-   `username` – your Linux user
-   `linux_host` – IP or hostname of the Linux machine
-   `/path/to/remote/directory` – destination folder on Linux

---

## Creating a Python Virtual Environment (venv) in Linux

1. Open a terminal.
2. Install the venv package (if needed):

    ```bash
    sudo apt install python3-venv
    ```

3. Navigate to your project directory.
4. Create the virtual environment:

    ```bash
    python3 -m venv myenv
    ```

    _Change `myenv` to whatever name you like._

5. Activate it:

    ```bash
    source myenv/bin/activate
    ```

---

## Finding a Process ID (PID) in Linux

1. Open a terminal.
2. List running processes:

    ```bash
    ps aux
    ```

3. Locate your process and note its **PID** (second column).
4. Or search directly:

    ```bash
    pgrep process_name
    ```

    _Replace `process_name` with the process you’re looking for._
