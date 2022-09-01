# API Deployment

## Django Settings Best Practices

### Different Django Configuration Approaches

* settings_local.py

  * Pros:

    * Secrets not in VCS

  * Cons:

    * settings_local.py is no in VCS, so you can lose some of your Django settings

    * Becasue it is in python, the file might have some non-obvious logic

    * You need to have settings_local.example to share default Django configs for devs

* Separate settings file for each environment

  * Pros

    * All environments are in VCS

    * It's easy to share between devs

  * Cons

    * You'll need to figure a way out to handle secret passwords and tokens

    * Inheritance of settings can be hard to trace and maintain

* Environmental variables

  * Pros

    * Configs are separate from the code

    * Environmental parity - you have the same code for all environments

    * No inheritance settings, and cleaner, more consistent code

    * There is theoretical grounding for using environment variables

  * Cons

    * You will need to handle sharing default configs between devs

## What is SSH

### Definition

SSH or Secure Shell Protocol is a remote administration protocol that allows users to access, control and modify their remote servers over the internet.

### Using SSH

You access SSH through your shell, and then create an SSH command with three distinct parts: the ssh key, the user, and the host. the ssh command lets the system know you want to open a remote terminal. The user represents the account that you would like to access. The host refers to the computer that you would like to access, which can either be an IP address or a domain name.

When accessing the remote terminal, SSH uses three separate kinds of encryption. This allows a very secure connection between you and the remote terminal.



