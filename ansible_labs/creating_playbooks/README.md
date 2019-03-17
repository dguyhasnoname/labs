# Creating playbooks

Plabooks mentioned here explains:
1) anisble playbooks structure
2) passing variables to playbooks
3) debugging in ansible
4) installing and customising a webserver.
5) jinja templating

##Exercises:

1. passing vairables in ansible: [passing vars](variable_passing.yml)

Command to run:
```
ansible-playbook -i host variable_passing.yml -e group_name=group1 -e user_name=user1
```
2. installing and running new webserver with default welcome page:[webserver installation](installing_webserver.yml)

Command to run:
```
ansible-playbook -i host installing_webserver.yml
```

3. debugging ouput in anisble: [debugging](debug_output.yml)

Command to run:
```
ansible-playbook -i host debug_output.yml 
```

4. adding a custom home page to webserver hosted: [custom page addition](custom_page_webserver.yml)

Command to run:
```
ansible-playbook -i host custom_page_webserver.yml
```

5. jinja templating: [jinja template](jinja_template_welcome_page.yml)

Command to run:
```
ansible-playbook -i host jinja_template_welcome_page.yml -e 'message="This page is dedicated to you"'
```