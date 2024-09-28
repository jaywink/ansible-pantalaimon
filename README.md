# Pantalaimon

Deploy a Pantalaimon using Docker.

https://github.com/matrix-org/pantalaimon

Targeting Ubuntu 20.04, contributions welcome for a larger set of platforms.

## Requirements

Developed and tested on Ansible 2.9.6.

## Usage

You can install this role from Ansible Galaxy with:

```bash
ansible-galaxy install jaywink.ansible_pantalaimon
```

Set the required variables for your play.

## Role Variables

```
# Required, no defaults
#pantalaimon_homeservers:
#  - name: myhomeserver
#    url: https://domain.tld
#    listen_port: "8009"

# Optional
pantalaimon_container_name: "{{ pantalaimon_name }}"
pantalaimon_container_labels: {}
pantalaimon_docker_image: matrixdotorg/pantalaimon:v0.10.5
pantalaimon_docker_networks: []
pantalaimon_log_level: Info
pantalaimon_name: "pantalaimon"
```

### Dependencies

None

## License

BSD

## Author Information

Jason Robinson / `@jaywink:federator.dev` / https://jasonrobinson.me
