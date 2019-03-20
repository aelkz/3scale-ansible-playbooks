### 3SCALE TOOLS

##### PRE-INSTALL REQUIREMENTS (mac osx)

```
brew tap jmespath/jmespath
brew install jp
brew upgrade && brew install jp
pip install jmespath-terminal
```

Create a new access-token inside 3Scale admin portal:

<img src="documentation/02.png" />

<img src="documentation/01.png" />

<img src="documentation/03.png" />

Copy the hosts.example content to your ansible/hosts file.

##### RUNNING

ansible-playbook roles/3scale-tools/main.yml -vvv -c paramiko -k --flush-cache --extra-vars "ansible_user=raphael"