# Try Out VS Cloud Environments: Python

This is a sample project that lets you try out VS Cloud Environments in a few easy steps.
   
## Things to try

This sample has been cloned into your VS Cloud Environment. You're able to work with it like you would any local code.

Some things to try:

1. **Install language extensions:**
  - Open `app.py`
  - Install the recommended Python extension
  - View the list of `Cloud Environment - Installed` extensions
    > Note: The Python extension has been installed in the remote environment
  - Reload VS Code
    > Note: VS Code automatically reconnects to your cloud environment

2. **Use Python:** 
  - Create a virtual environment: `virtualenv env` and select it for the folder workspace
  - Activate the environment: `cd env/bin` followed by `. activate`
  - Install Flask" `pip install flask` 

3. **Edit code:**
   - Open `app.py`
   - Try adding some code and check out the IntelliSense

4. **Terminal:** 
  - From the terminal run `python --version`
    > Note: Python is not installed on the local machine, yet you're able to use it! 
  - Type other Linux commands (`uname`, `ls`, etc.) to interact with the underlying environment
    > Note: The local machine is Windows, yet you're able to issue Linux commands! 
  - Run `python` to issue commands in the Python interpreter (`print("Hi mom")`, `7 * 6`, etc.) 
    > Note: Use `exit()` to leave the Python interpreter

5. **Build, Run, and Debug:**
   - Open `app.py`
   - Add a breakpoint (e.g. on line 9)
   - Change the message in `static\index.html` to "Hello {your name} from Python!"
   - Press F5 to launch the app
   - Once the breakpoint is hit, try hovering over variables (e.g. the app variable on line 7), examining locals, and more.
   - Continue, then open a local browser and go to `http://localhost:9000` and note you can't connect to the server

5. **Forward port:**
   - Stop debugging and remove the breakpoint.
   - Open `.vscode/launch.json`
   - Change the server port to 5000 on line 20 (`"--port","5000"`)
   - Press F5 to launch the app in the container.
   - Run the **Cloud Environments: Forward Port from Environment...** command
     - Enter port 5000
     - Name it anything you'd like
     - View the forwarded ports in the Environment Details panel
   - Open http://localhost:5000/ and show the booth attendant the running site
   
6. **Finish**
  - Complete steps 5-7 on the Challenge Worksheet
