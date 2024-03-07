# setup-ansible
A GitHub Workflow action to setup Ansible.

# Usage

```yaml
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
    
      - name: "Install Ansible"
        uses: ./ 
        with:
          version: "9.3.0"

      - name: "Print Ansible version"
        run: ansible-playbook --version

```
