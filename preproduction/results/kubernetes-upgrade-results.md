Nombre de la asignación

Participantes

    Nombre: 
      Luis Angel Juarez Rodriguez
      Alberto Martinez Facundo
      Zinhue Gonzalez 
      JESUS JULIAN RAMIREZ MORENO
      Angel Juan Martínez García 
      Diego Alejandro Trejo Angelino
      Vicente Eduardo Escareño Lopez
      JOSÉ DOMINGO LÁZARO RAMÍREZ


Actividades

    Actividad

Comandos

    Comandos

Recursos externos

    Recurso externo

Artifactos

    Anexar artifactos al directorio de respuesta

[54.219.51.220] (kubernetes-admin@kubernetes:N/A) k8s@preprod1 ~
$ kubectl version
WARNING: This version information is deprecated and will be replaced with the output from kubectl version --short.  Use --output=yaml|json to get the full version.
Client Version: version.Info{Major:"1", Minor:"26", GitVersion:"v1.26.0", GitCommit:"b46a3f887ca979b1a5d14fd39cb1af43e7e5d12d", GitTreeState:"clean", BuildDate:"2022-12-08T19:58:30Z", GoVersion:"go1.19.4", Compiler:"gc", Platform:"linux/amd64"}
Kustomize Version: v4.5.7
Server Version: version.Info{Major:"1", Minor:"26", GitVersion:"v1.26.0", GitCommit:"b46a3f887ca979b1a5d14fd39cb1af43e7e5d12d", GitTreeState:"clean", BuildDate:"2022-12-08T19:51:45Z", GoVersion:"go1.19.4", Compiler:"gc", Platform:"linux/amd64"}


[54.219.51.220] (kubernetes-admin@kubernetes:N/A) k8s@preprod1 ~
$ kubectl version
WARNING: This version information is deprecated and will be replaced with the output from kubectl version --short.  Use --output=yaml|json to get the full version.
Client Version: version.Info{Major:"1", Minor:"26", GitVersion:"v1.26.0", GitCommit:"b46a3f887ca979b1a5d14fd39cb1af43e7e5d12d", GitTreeState:"clean", BuildDate:"2022-12-08T19:58:30Z", GoVersion:"go1.19.4", Compiler:"gc", Platform:"linux/amd64"}
Kustomize Version: v4.5.7
Server Version: version.Info{Major:"1", Minor:"27", GitVersion:"v1.27.0", GitCommit:"1b4df30b3cdfeaba6024e81e559a6cd09a089d65", GitTreeState:"clean", BuildDate:"2023-04-11T17:04:24Z", GoVersion:"go1.20.3", Compiler:"gc", Platform:"linux/amd64"}



[54.219.51.220] (kubernetes-admin@kubernetes:N/A) k8s@preprod1 ~
$ kubectl get nodes -o wide
NAME       STATUS   ROLES           AGE   VERSION   INTERNAL-IP     EXTERNAL-IP   OS-IMAGE             KERNEL-VERSION    CONTAINER-RUNTIME
preprod1   Ready    control-plane   40m   v1.27.0   172.31.10.175   <none>        Ubuntu 22.04.2 LTS   5.19.0-1029-aws   containerd://1.6.22
preprod2   Ready    <none>          40m   v1.27.0   172.31.4.171    <none>        Ubuntu 22.04.2 LTS   5.19.0-1029-aws   containerd://1.6.22
preprod3   Ready    <none>          40m   v1.27.0   172.31.6.5      <none>        Ubuntu 22.04.2 LTS   5.19.0-1029-aws   containerd://1.6.22
