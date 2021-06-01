# Descomplicando Ansible

Projeto do treinamento descomplicando Ansible + AWS

## Fases do projeto
```
- Provisioning -> Cria as instancias/vms para o nosso cluster;
- Install_k8s -> Criação do cluster;
- Deploy_app -> Deploy de uma aplicação exemplo;
- Extra -> ...

```

## Observações
Arquivo de hosts:
```
[k8s-master]
hostip-or-dns

[k8s-workers]
hostip-or-dns

[k8s-workers:vars]
K8S_MASTER_NODE_IP=hostip-or-dns
K8S_API_SECUREPORT=6443

[all:vars]
ansible_python_interpreter=python3
```
Dependências modulo k8s ansible

pip3

Pacotes pip utilizado:
```
- openshift==0.8.6
- PyYAML==5.4.1
- kubernetes==8.0.2
```
