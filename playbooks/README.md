# Playbooks
Hier ist die Reihenfolge enthalten, in der die Files ausgeführt werden müssen, um Kubernetes aufzusetzen.

## Meilenstein 1
- Zuerst kommen die Files [master_config.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/master_config.yaml) und [worker_config.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/worker_config.yaml). Da spielt es keine Rolle, da beide die jeweiligen Nodes (Master und Worker) konfigurieren.
- Danach kommt das File [install_containerd.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/install_containerd.yaml). Dieses installiert und konfiguriert Containerd.
- Als nächstes File kommt [install_kubernetes.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/install_kubernetes.yaml). Das File installiert Kubernetes samt Abhängigkeiten.
- Als viertes File kommt [configure_cluster.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/configure_cluster.yaml). Das initialisiert und konfiguriert den Cluster.
- Mit dem File [join_nodes.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/join_nodes.yaml), können wir dann bereits die Worker Nodes zum Cluster hinzufügen.
- Das letzte File wäre [networkplugin.yaml](https://github.com/nathanaugsburger/abschlussprojekt_zli/blob/main/playbooks/networkplugin.yaml). Damit installieren wir noch ein Netzwerk Plugin.

Wenn man die Files in der richtigen Reihenfolge ausgeführt hat, sollte das Cluster samt Nodes jetzt laufen.

Files die nicht in dieser Auflistung enthalten sind werden nicht direkt benötigt. Eine Ausnahme ist das Inventory File. Dieses enthält die Zielhosts.
