# MouzWheeler
A simple script that duplicates mouse wheel up and down events - so your scrolling speed will be faster under Linux. This applies only for the first input device that is a mice and has a wheel. 

## Installation - Automatic
Download the whole repo.```chmod +x installer; ./installer``` to run the installer. 

## Installation - Manual
The app uses only one external python package dependency: ```evdev```. In order to run the package installation yourself, execute:
```bash
pip install -r requirements.txt
```
**AS ROOT**: 
```python
# Copy over the files from the ```_``` directory.
cp -a _/* /
# Reload new systemd service unit files
systemctl daemon-reload
# enable+start the service
systemctl enable mouzwheeler
systemctl start mouzwheeler
# enjoy!
```

## Configuration
The app related configuration can be found under ```/etc/default/mouzwheeler```.
