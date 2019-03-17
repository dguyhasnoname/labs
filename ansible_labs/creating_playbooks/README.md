# Creating playbooks

Exercises:
> passing vairables in ansible: ![passing vars](variable_passing.yml)
```
ansible-playbook -i host variable_passing.yml -e group_name=group1 -e user_name=user1
```
> installing and running new webserver with default welcome page: ![webserver installation](installing_webserver.yml)
> debugging ouput in anisble: ![debugging](debug_output.yml)
> adding a custom home page to webserver hosted: ![custom page addition](custom_page_webserver.yml)
> jinja templating: ![jinja template](jinja_template_welcome_page.yml)

```
ansible-playbook -i host jinja_template_welcome_page.yml -e 'message="This page is dedicated to you"'
```