# Clockweb

**Frontend**: Simple web page showing us the date in human readable form.

**Backend**: Returns unix timestamp when accessing to `/clock` endpoint.

## Deployment

In order for you to deploy this webapp successfuly you need first:

1. Clone this repo.
1. Update your server's IP address in the inventory.
1. And last but not least, execute the following commands:

```bash
alias ansible-playbook="docker run -ti --rm -v $(pwd):/apps -w /apps alpine/ansible ansible-playbook"
ansible-playbook backend.yml
```
