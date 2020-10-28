# CTFd

This role sets up CTFd with HTTPS using letsencrypt.


## Role Variables

- `domain`: Domain name of your CTFd (Buying and DNS configuration
  left as an exercise).
- `owner`: Unix user for this service.
- `ctfd_version`: Tag/version to install, defaults to `master`.


## Example Playbook

```yaml
- hosts: ctfd
  roles:
   - ctfd
  vars:
    letsencrypt_email: coucou@example.com
    domain: ctfd.example.com
    version: "3.1.1"
    secret_key: "some_random_string"
```


### License

MIT


### Author Information

Julien Palard — https://mdk.fr
