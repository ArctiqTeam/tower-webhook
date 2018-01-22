# Custom Webhook for Ansible Tower

The main purpose of this project is to provide an automated Ansible installer for a custom webhook that works with Ansible Tower.  The webhook can be used in conjunction with GitHub (more providers planned to be added later) to allow webhooks in Git to intitiate Tower project (and inventory if hosted inside) updates upon commit/push to a repository.

## Built With

The project consists of an Ansible playbook to install and configure the webhook.  The webhook binary is provided by [Hookdoo](https://github.com/adnanh/webhook)

## Requirements

 1. A host that is accessible from Git (currently over Port 9000)
 2. Ansible Tower server (currently only a single Tower server is supported) accessible from the webhook target

## Installing

 * Customize the vars.yml file accordingly
 * Customize the hosts file as needed - this is the host that will run the webhook
 * Run the playbook

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* [Hookdoo](https://github.com/adnanh/webhook)
