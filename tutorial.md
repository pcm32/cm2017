# Cloud basics, with PhenoMeNal

This tutorial is divided in two parts: 
- Cloud 101 slides and demos to give a general understanding and vocabulary of cloud computing elements (30 minutes).
- PhenoMeNal overview slides and demos of the PhenoMeNal Portal, deployment and public instance (1 hour).

## Cloud 101 Slides

Duration: 25 minutes

Slides available [here](https://drive.google.com/open?id=0B3GjpBpPCNBcMEpfT1ZBMmtqS1E).

Topics:
- Show of hands
- What is cloud computing
- IaaS, PaaS, etc
- Public, private and hybrid cloud providers
  - Heterogeneity within (zones) and inter cloud providers
- Building blocks:
  - Virtual Machines
  - Containers
  - Infrastructure as code
- PhenoMeNal as a use case


## OpenStack and Amazon dashboard demo

Duration: 5 minutes (running 30 min.)

A quick walk through inside a cloud provider's web dashboard/control panel, to give an idea of what you get.

### OpenStack

- Show volumes
- Show flavours
- Show instances
- Show networks

## PhenoMeNal Slides

Duration: 15 minutes (running 45 min.)

- Similar slides as used for Metabolomics Conference, spending more time in the use cases.

## PhenoMeNal Portal practical

Duration: 20 minutes (running 65 minutes)

- As done at the SAB and Stakeholder demo, inviting users to try it as we go.
- Login / Register
- Show around App Library, Help, and how to deploy.
- Show an existing deployment, quickly accessing Galaxy, Jupyter and the spooky dashboard.

## PhenoMeNal Public instance/deployed demo

Duration: 20 minutes (running 1:25)

- Show how to execute the Fluxomics workflow on the public instance or a deployed instance, as done during the SAB/stakeholder meeting.
- Possibly showing the video instead of presenting directly, and then showing the interactivity of the visualization.

## Closing remarks

Duration: few minutes

- Invite to interact during the course and beyond:
  - To show us how does your analysis pipeline looks like, and look into whether we have all the elements for it in PhenoMeNal, or whether we would need some additions.
  - If you have an interest in using containers for your research, or any other technology mentioned.




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

## Bonus on-the-go: PhenoMeNal on your laptop

- For those who installed minikube and helm on their machines [as requested](installation_requests.md), instructions on how to lift our Galaxy instance on their own machines will be given:

  - Download this config file phenomenal-galaxy-laptop.yaml.

```
$ minikube start 
$ helm repo add galaxy-kubernetes
$ helm install -f phenomenal-galaxy-laptop.yaml --version 0.3.1 galaxy-kubernetes/galaxy
```
  - On your browser, visit http://192.168.99.100:30700/

## Virtual Machines and Containers demo

Duration: 15 minutes - Cancelled as too technical.

- Show how a virtual machine can be started, with VirtualBox, making a note on how much it takes to start.
  - and how it can be provisioned with cloud-config. 
- Show a dockerfile and the output of when it was created (use existing logs in CI to avoid waits)
  - Show how quickly you can get into the container
  - Show how easily you can run things inside the container from the outside.

  
