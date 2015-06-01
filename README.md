# ansible-role-java

Installs java from ppa:webupd8team, this role requires license acception (unlike [this one](https://github.com/mhamrah/ansible-java8)).

## Variables

Here're the variables and there default values:

```yaml
java_installer_version: 8
i_do_accept_oracle_binary_code_license_agreement_for_the_java_se_platform_products_and_javafx_please_skip_the_prompt: no
```

Note that prompts [do not work](https://github.com/ansible/ansible-modules-core/issues/656) with vagrant (so accept license with a variable).

This role is tested with java 8 and ubuntu 14.04.

For more details about debconf read [here](http://askubuntu.com/a/190674).
