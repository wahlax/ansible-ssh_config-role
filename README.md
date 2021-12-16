# SSH config with Ansible

Role for configuring ssh. Entries are validated.

## Optional Parameters

 * `sshconfig_custom_sshd_config` - additional configs with key and value  

```
sshconfig_custom_sshd_config:
  - key: "PasswordAuthentication"
    value: "yes"
```

## Testing

Credit: Tested with vagrant image from [@geerlingguy's Ansible for Devops](https://github.com/geerlingguy/ansible-for-devops)

Run the following from the test directory:

### Initial Install
```
vagrant up
```

### Reapply provisioning
```
vagrant provision
```

