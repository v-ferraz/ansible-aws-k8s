## Arquivo hosts para provisionar as instâncias ec2

O ansible irá executar o playbook localmente para criar as instâncias em cloud. Após concluído, será adicionar os endereços ips público e privado nas seções correspondentes.

```
[local]
localhost ansible_connection=local ansible_python_interpreter=python3 gather_facts=false

[kubernetes]

[kubernetes-privateip]
```
