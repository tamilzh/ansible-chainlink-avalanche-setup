# reddev infrastructure automation repository
Setup requirements:
1. Get Vultr.com API key from https://my.vultr.com/settings/#settingsapi
2. Create file at ~/.vultr.ini and fill in your API key like so:
```
[reddev]
key = quertyuiop123456789
timeout = 60
 ```

## Developement server creation
1. Run `ansible-playbook -i inventory tasks/createvultrvps.yml`
2. Follow directions to create new developement server in Vulr
3. Run `ansible-playbook -i inventory tasks/provision.yml`
4. Follow directions to provision the newly created developement server