# Useful Linux Commands and Tips

---

## How to Transfer Files from Windows to Linux using SCP (Secure Copy Protocol)

1. Open a terminal on your **Linux** machine.
2. Copy a file from Windows to Linux:
    ```bash
    scp /path/to/local/file username@linux_host:/path/to/remote/directory
    ```

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

## How to create a requirements.txt file in Linux

1. Open a terminal.
2. Navigate to your project directory.
3. Activate your virtual environment if you have one:

    ```bash
    source myenv/bin/activate
    ```

    _Replace `myenv` with your virtual environment name._

4. Run the following command to create a requirements.txt file:

    ```bash
    pip freeze > requirements.txt
    ```

    _This will list all installed packages and their versions in the current environment._

---

## How to install packages from requirements.txt in Linux

1. Open a terminal.
2. Navigate to your project directory.
3. Activate your virtual environment if you have one:

    ```bash
    source myenv/bin/activate
    ```

    _Replace `myenv` with your virtual environment name._

4. Ensure you have a `requirements.txt` file in your project directory.

    _If you don't have one, you can create it using the previous section's instructions._

5. Run the following command:

    ```bash
    pip install -r requirements.txt
    ```

---

## How to run a Python Script in Linux

1. Open a terminal.

    _Ensure you have activated your virtual environment if you are using one._

2. Navigate to the directory containing your script.
3. Run the script using Python 3:

    ```bash
    python3 script_name.py
    ```

    _Replace `script_name.py` with the name of your Python script._

---

## How to run a Python Script and keep it running in the background

1. Open a terminal.

    _Ensure you have activated your virtual environment if you are using one._

2. Navigate to the directory containing your script.
3. Run the script in the background:

    ```bash
    nohup python3 script_name.py &
    ```

    _Replace `script_name.py` with your script's name._

---

## How to see the output of a Python script running in the background

1. Open a terminal.
2. Navigate to the directory where you ran the script.
3. Check the output file:

    ```bash
    cat nohup.out
    ```

    _This file contains the output of your script._

4. If you want to see the output in real-time, you can use:

    ```bash
    tail -f nohup.out
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

---

## How to Kill a Process in Linux using PID

1. Open a terminal.
2. Use the `kill` command with the PID:

    ```bash
    kill PID
    ```

    _Replace `PID` with the actual process ID._

## Useful VSCode Shortcuts

-   **Move Line Up/Down**: `Alt + Up/Down Arrow`
-   **Add multiple cursors**: `Ctrl + Alt + Click` or `Ctrl + Alt + Up/Down Arrow`
-   **Delete Line**: `Ctrl + Shift + K`
-   **Comment/Uncomment Line**: `Ctrl + /`
-   **Select current line**: `Ctrl + L`
-   **Navigate to a specific line**: `Ctrl + G`
-   **Go to Definition**: `F12`
-   **Select all occurrences of a operation**: `Ctrl + F2`
-   **Trim Trailing Whitespace**: `Ctrl + K` then `Ctrl + X`
-   **Copy Line Up/Down**: `Shift + Alt + Up/Down Arrow`
-   **Open Command Palette**: `Ctrl + Shift + P`
-   **Open Markdown Preview**: `Ctrl + Shift + V`
