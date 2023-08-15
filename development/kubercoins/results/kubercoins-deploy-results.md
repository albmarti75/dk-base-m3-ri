Nombre de la asignación

Participantes

    Nombre: Hector Israel Castro
    Nombre: Alberto Martinez Facundo

Actividades

    Actividad: Development/Deploy kubecoins

Comandos

    Comandos: kubectl apply -f ~/container.training/k8s/dockercoins.yaml
              kubectl get svc webui
              curl <ClusterIP

Recursos externos

    Recurso externo

Artifactos

    Anexar artifactos al directorio de respuesta

 [54.191.218.245] (kubernetes-admin@kubernetes:N/A) k8s@test1 ~
$ kubectl get services
NAME         TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)        AGE
hasher       ClusterIP   10.97.72.236     <none>        80/TCP         27m
kubernetes   ClusterIP   10.96.0.1        <none>        443/TCP        138m
redis        ClusterIP   10.103.246.246   <none>        6379/TCP       27m
rng          ClusterIP   10.97.206.48     <none>        80/TCP         27m
webui        NodePort    10.109.240.124   <none>        80:31936/TCP   27m

[54.191.218.245] (kubernetes-admin@kubernetes:N/A) k8s@test1 ~
$ kubectl get pods
NAME                      READY   STATUS    RESTARTS   AGE
hasher-65db859b66-zfc72   0/1     Pending   0          19m
redis-6ff7cd7598-56vnx    0/1     Pending   0          19m
rng-5bd86c8566-2r75f      0/1     Pending   0          19m
webui-6969bf568c-66274    0/1     Pending   0          19m
worker-6bbc87d469-p4sd2   0/1     Pending   0          19m
