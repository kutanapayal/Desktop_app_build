# Desktop_app_ubuntu_build

**To Install Dependancies Run This Command**

      <sub>pip3 install -r requirements.txt </sub>
      
 **To Run The Script**
      <sub>python3 time_tracker.py</sub>

**To Create Ubuntu Build Use the Following Command**

    <sub>pyinstaller --onefile --noconsole --icon="icon.ico" --add-data="index.ui:." --add-data="login.ui:." --add-data="credentials.json:." --add-data="processing.gif:." --add-data="logout.xpm:." --add-data="user_icon.xpm:." time_tracker.py</sub>
