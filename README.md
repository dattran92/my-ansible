# MY ANSIBLE

### Requirement

- ansible
- sshpass (if you are using password to connect to your server)

```
  brew install https://raw.githubusercontent.com/kadwanev/bigboybrew/master/Library/Formula/sshpass.rb
```

### Install dependencies (ansible galaxy)

```
  ansible-galaxy install [packages]
```

### Run playbook

```
ansible-playbook -i hosts -v main.yml --ask-sudo-pass
```
