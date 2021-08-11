# Ansible-Yum-Apache-Handlers-Configuration

## 📌Restarting HTTPD Service is not idempotence in nature and also consume more resources suggest a way to rectify this challenge in Ansible playbook

**What is Handlers in Ansible?**

1. Handlers are just like normal tasks in an Ansible playbook but they run only when if the Task contains a “notify” directive. It also indicates that it changed something.

2. By default, handlers run after all the tasks in a particular play have been completed. This approach is efficient, because the handler only runs once, regardless of how many tasks notify it. For example, if multiple tasks update a configuration file and notify a handler to restart Apache, Ansible only bounces Apache once to avoid unnecessary restarts.

3. Handlers have the capability if u changed something, first, you need to notify it and after use in the name of a handler.

In this way, Problem has been solved...

## Blog URL: https://www.linkedin.com/pulse/restarting-httpd-service-idempotence-nature-also-consume-suraj-warbhe/
