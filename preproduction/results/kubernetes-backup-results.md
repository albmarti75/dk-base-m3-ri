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
