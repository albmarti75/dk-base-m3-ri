Nombre de la asignación

Participantes

    Nombre: Docker Coins

Actividades

    Actividad: Kubernetes Backup

Comandos

    Comandos: 

Recursos externos

    Recurso externo: 

Artifactos

    Anexar artifactos al directorio de respuesta


$ docker run --rm --net host -v $PWD:/vol \
    -v /etc/kubernetes/pki/etcd:/etc/kubernetes/pki/etcd:ro \
    -e ETCDCTL_API=3 k8s.gcr.io/etcd:3.3.10 \
    etcdctl --endpoints=https://[127.0.0.1]:2379 \
            --cacert=/etc/kubernetes/pki/etcd/ca.crt \
            --cert=/etc/kubernetes/pki/etcd/healthcheck-client.crt \
            --key=/etc/kubernetes/pki/etcd/healthcheck-client.key \
            snapshot save /vol/snapshot
Unable to find image 'k8s.gcr.io/etcd:3.3.10' locally
3.3.10: Pulling from etcd
90e01955edcd: Pull complete 
6369547c492e: Pull complete 
bd2b173236d3: Pull complete 
Digest: sha256:17da501f5d2a675be46040422a27b7cc21b8a43895ac998b171db1c346f361f7
Status: Downloaded newer image for k8s.gcr.io/etcd:3.3.10
Snapshot saved at /vol/snapshot




[54.219.51.220] (kubernetes-admin@kubernetes:N/A) k8s@preprod1 ~
$ ls -la
total 2772
drwxr-x--x 6 k8s  users    4096 Aug 15 02:14 .
drwxr-xr-x 4 root root     4096 Aug 15 02:03 ..
-rw-r--r-- 1 k8s  users     220 Jan  6  2022 .bash_logout
-rw-r--r-- 1 k8s  users    4271 Aug 15 02:05 .bashrc
drwx------ 2 k8s  users    4096 Aug 15 02:14 .cache
-rw------- 1 k8s  users     487 Aug 15 02:19 .history
drwxr-xr-x 6 k8s  users    4096 Aug 15 02:05 .krew
drwxr-xr-x 2 k8s  root     4096 Aug 15 02:05 .kube
-rw-r--r-- 1 k8s  users     807 Jan  6  2022 .profile
drwxr-xr-x 2 k8s  users    4096 Aug 15 02:03 .ssh
-rw-r--r-- 1 k8s  users     491 Aug 15 02:03 .tmux.conf
-rw-r--r-- 1 k8s  users      96 Aug 15 02:03 .vimrc
-rw-r--r-- 1 root root  2781216 Aug 15 02:14 snapshot
