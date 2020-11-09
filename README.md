# Ansible Role: Jenkins CI

Installs Jenkins on RHEL/CentOS and Debian/Ubuntu servers.

## Example Playbook

```yaml
- hosts: jenkins
  become: true
  
  vars:
    jenkins_hostname: jenkins.example.com
    java_packages:
      - openjdk-8-jdk

  roles:
    - role: ./roles/jenkins
```

Note that `java_packages` may need different versions depending on your distro (e.g. `openjdk-11-jdk` for Debian 10, or `java-1.8.0-openjdk` for RHEL 7 or 8).

## License

MIT 

## Author Information

This role was created in 2020 by [Arbaz Khan]
