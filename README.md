# abschlussprojekt_zli
## Thema
In meinem Projekt geht es darum, mit Ansible alles rund um Kubernetes zu automatisieren. Mithilfe von Ansible will ich eine Kubernetes Umgebung erstellen und auf dieser dann Applikationen deployen, natürlich ebenfalls mit Ansible. Ebenfalls will ich wissen, wie ich mithilfe von Ansible möglichst schnell eine VM mit spezifischen Anforderungen bereitstellen kann. 
## Inhalt
In diesem Repository werde ich alle meine Dateien des Abschlussprojektes hochladen.
Folgende Dateien sind in diesem Repo enthalten:
- Ansible Playbooks
- YAML-Files für Deployment
## Playbooks
### Docker Setup
Das Playbook [install_docker.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/install_docker.yaml)
enthält die Installation der Abhängigkeiten, von Docker selbst und das Hinzufügen des gewünschten Benutzers zur Docker Gruppe.
### Kubernetes Setup
Das Playbook [install_kubernetes.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/install_kubernetes.yaml)
enthält die Installation der Abhängigkeiten, das Deaktivieren des Swap, so wie die Installation der Kubernetes Pakete kubeadm, kubectl und kubelet.
