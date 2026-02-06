## 使用 GitHub 仓库

```
~]# cat > requirements.yml << EOF
---
roles:
  - src: https://github.com/dengyouf/ansible-galaxy-initsys.git
    scm: git
    version: main
EOF
```

```
~]# ansible-galaxy install -r requirements.yml

```

- ` ansible-playbook -i ~/.ansible/roles/ansible-galaxy-initsys/tests/inventory ~/.ansible/roles/ansible-galaxy-motd/tests/test.yml`
