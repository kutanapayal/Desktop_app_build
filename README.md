# Desktop_app_ubuntu_build

**To Install Dependancies Run This Command**

     pip3 install -r requirements.txt
      
 **To Run The Script**
 
      python3 time_tracker.py

**To Create Ubuntu Build Use the Following Command**

    pyinstaller --onefile --noconsole --icon="icon.ico" --add-data="index.ui:." --add-data="login.ui:." --add-data="credentials.json:." --add-data="processing.gif:." --add-data="logout.xpm:." --add-data="user_icon.xpm:." time_tracker.py
