# Configure a Cubieboard as SixXS tunnel endpoint

Set up the tunnel with SixXS and use radvd to announce the network

Tested on a Cubieboard with Armbian https://www.armbian.com (Ubuntu Xenial Kernel 4.7.3)

## Run the Ansible playbook

Run the playbook from the cubieboard

```
apt-get install ansible
git clone https://github.com/zioproto/ansible-cubieboard-sixxs-gw.git
cd ansible-cubieboard-sixxs-gw
mkdir roles
git clone https://github.com/zioproto/ansible-aiccu roles/aiccu
cp vars.yaml.template vars.yaml
vim vars.yaml
ansible-playbook main.yaml
```
