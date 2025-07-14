# Infra Templates

Reusable Jinja2 and Packer templates for GitOps infrastructure provisioning.

## Structure

- `namespaces/` – OCP project templates
- `vms/` – KubeVirt VM manifests
- `osimages/` – Packer-based machine image builds
- `misc/` – Generic infra types (DNS, certs, etc.)

## Usage

Each template accepts `{{ variable }}` substitutions from the API processor. Templates can be rendered using Jinja2 before committing to tenant Git repositories.

## Customization

- Use `custom.yaml.j2` to create your own pattern.
- Override labels, annotations, resources as needed.
- test
