# Desktop_app_ubuntu_build

**You Can Install Dependancies By This Command**

<sub>pip3 install -r requirements.txt </sub>

**To Create Ubuntu Build Use the Following Command**

pyinstaller --onefile --noconsole --icon="icon.ico" --add-data="index.ui:." --add-data="login.ui:." --add-data="credentials.json:." --add-data="processing.gif:." --add-data="logout.xpm:." --add-data="user_icon.xpm:." time_tracker.py
