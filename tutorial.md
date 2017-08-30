# Cloud metabolomics tutorial

## Show of hands

- Who has spinned a VM.
- Who knows what a container is.
- Who has used any cloud services beyond dropbox.

## Cloud 101 Slides - 20 minutes

Topics:
- What is cloud computing
- Public, private and hybrid cloud providers
  - Mention some particular ones.
  - Heterogeneity within (zones) and inter cloud providers
- Academic clouds
- IaaS, PaaS, etc
  - Turn key solutions.
- Building blocks:
  - Virtual Machines
  - Containers
  - Infrastructure as code
    - Alternatives for hardware and software provisioning
  - Orchestration
- PhenoMeNal as a use case
- Discuss the administrative intrincancies of getting a paid cloud account through academic institutions.
  - If the intend to use cloud providers in the future, they need to start talking to their finance/admin layer to understand how this can be done.

## Virtual Machines and Containers demo

- Show how a virtual machine can be started with vagrant
  - and how is provisioned with cloud-config. 
- Start the VM as well with VirtualBox, making a note on how much it takes to start.
- Create a dockerfile with the same software
  - Show how quickly you can get into the container
  - Show how easily you can run things inside the container from the outside, as opposed to the VM.

## OpenStack dashboard demo

- Show instances
- Show flavours
- Show networks
- Talk about amazon and Google dashboard

## Infrastructure as a code

### Hardware provisioning: terraform

- Explain again what is Terraform.
- Show an example plan, deployment and destroy with terraform.
- Ask them to write a terraform file that:
  - Creates terraform main.tf file (everything else provided) that provisions 1 machine with at least 2 GB of RAM and that has attached a 5 GB external disk.
    - Students are asked to look into the Terraform documentation for OpenStack. After 10 minutes, we give them the solutions on where they should have looked.
  - Ask students to run the solution code (or theirs) on terraform katacoda ([ ] setup katacoda).
- Show an example ansible script that installs mzml2isa
- Go through the PhenoMeNal terraform script for OpenStack.

### Software provisioning

- Explain what Ansible is.
- Show the Ansible documentation for a few modules.
  - Copy a file
  - Change a file permissions
  - Execute a shell command
  - Install a package
- Show a set of ansible tasks from [PhenoMeNal](https://github.com/phnmnl/container-galaxy-k8s-runtime/blob/develop/ansible/set-galaxy-config-values.yaml)




  
