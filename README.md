# DEVELOPMENT

1. install python 3.11 (tested) virtual env  
    
    `py -3.11 -m venv .`

2. enable virtual env 
    
    `Scripts\activate.bat`

3. install requirements 

    `pip install -r requirements.txt`

4. make your logic after `# your logic here` comment


# DEPLOYMENT (require administrator privilges)

1. make exe of service 
    
    `pyinstaller --onefile --hidden-import win32timezone service.py`

2. install service

    `dist\service.exe install`

3. start service

    `dist\service.exe start`

4. stop service

    `dist\service.exe stop`

5. remove service

    `dist\service.exe remove`

6. install with autostart:

    `dist\service.exe --startup delayed install`