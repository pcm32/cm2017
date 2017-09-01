# Components to install

The following directions will give you links to install components for the optional task of trying to lift PhenoMeNal on your own laptop, which could enable you to try lightweight analysis. If you go through it, you should end up with the following components installed:

- VirtualBox (or another hypervisor). Many of you might already have this.
- Minikube
- kubectl
- Helm

# Minikube

From its website:

"Minikube is a tool that makes it easy to run Kubernetes locally. Minikube runs a single-node Kubernetes cluster inside a VM on your laptop for users looking to try out Kubernetes or develop with it day-to-day."

Please download and install minikube for your platform following directions from [this link](https://kubernetes.io/docs/tasks/tools/install-minikube/). This will take you through the installation of necessary dependencies, like VirtualBox (which you might already have installed) and kubectl, the interface.

# Helm

Helm is a package manager for Kubernetes. We use it to automate and simplify the deployment of PhenoMeNal components. Installation instructions for macOS and linux can be found [here](https://github.com/kubernetes/helm#install). For Windows, it can be installed following [this directions](https://github.com/kubernetes/helm/releases/tag/v2.5.1).




