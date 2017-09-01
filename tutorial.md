# Cloud basics, with PhenoMeNal

This tutorial is divided in two parts: 
- Cloud 101 slides and demos to give a general understanding and vocabulary of cloud computing elements (40 minutes).
- PhenoMeNal overview slides and demos of the PhenoMeNal Portal, deployment and public instance (50 minutes).

## Show of hands

- Who has spinned a VM.
- Who knows what a container is.
- Who has used any cloud services beyond dropbox.

## Cloud 101 Slides

Duration: 15 minutes

Topics:
- What is cloud computing
- Academic clouds
- IaaS, PaaS, etc
  - Turn key solutions.
- Building blocks:
  - Public, private and hybrid cloud providers
    - Mention some particular ones.
    - Heterogeneity within (zones) and inter cloud providers
  - Virtual Machines
  - Containers
  - Infrastructure as code
    - Hardware and software provisioning
  - Orchestration
- PhenoMeNal as a use case
- Mention the administrative intrincancies of getting a paid cloud account through academic institutions.
  - If the intend to use cloud providers in the future, they need to start talking to their finance/admin layer to understand how this can be done.

## Virtual Machines and Containers demo

Duration: 15 minutes

- Show how a virtual machine can be started, with VirtualBox, making a note on how much it takes to start.
  - and how it can be provisioned with cloud-config. 
- Show a dockerfile and the output of when it was created (used logs in CI)
  - Show how quickly you can get into the container
  - Show how easily you can run things inside the container from the outside, as opposed to the VM.

## OpenStack and Amazon dashboard demo

Duration: 10 minutes

A quick walk through inside two cloud provider's web dashboard.

### OpenStack

- Show instances
- Show flavours
- Show networks
- Talk about amazon and Google dashboard

### Amazon

- Show EC2

## PhenoMeNal Slides

Duration: 15 minutes

- Similar slides as used for Metabolomics Conference, spending more time in the use cases.

## PhenoMeNal Portal demo

Duration: 20 minutes

- As done at the SAB and Stakeholder demo
- Login / Register
- Show around Help, Wiki and how to deploy.

## PhenoMeNal Public instance/deployed demo

Duration: 10 minutes

- Show how to execute the Fluxomics workflow on the public instance or a deployed instance.




# Other ideas, not to be included currently:

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




  
