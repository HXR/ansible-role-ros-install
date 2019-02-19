# Ansible ROS Install Role
This is a role to help guide the installation of [ROS (Robot Operating System)](https://www.ros.org/)  

## Dependencies
None  

## Variables
Look in [defaults/main.yml](defaults/main.yml) for role variables  

### Variable Configurations
There are some pre-made configuration files for various Ubuntu and Debian distributions in the `vars` folder  

## Example Playbook
```yaml
- vars_files:
    - vars/ubuntu-16.04.yml
  vars:
    - ros__package: ros-base
  roles:
    - mynameiscosmo.ros-install
```

## TODO
The following is a rough todo list for this repo  
- [ ] ROS Distro detection  
    - [ ] Notify if not supported  
    - [ ] Automatically select ROS version if supported  
    - test 404 error? : http://packages.ros.org/ros/ubuntu/dists/  
- [ ] Tests  
    - [ ] Coverage  
    - [ ] Repo key verification  
- [ ] Evaluate buildling from source  
  - [ ] building ros desktop + packages from source  
  - [ ] building with Python3  
- [ ] Documentation  
    - [ ] yaml2rst  

## License
BSD / MIT  

## Resources
This Ansible Role tries to follow [DEP2 - DebOps code standards](https://docs.debops.org/en/master/dep/dep-0002.html)  
