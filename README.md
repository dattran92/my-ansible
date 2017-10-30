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

### Configuration

- To add your own configuration, add `local` file nested in `server` folder in `group_vars

```
group_vars
  server
    local
```

### Run playbook

- If you need to enter sudo password

```
ansible-playbook -i hosts -v main.yml --ask-sudo-pass
```

- otherwise

```
ansible-playbook -i hosts -v main.yml
```
