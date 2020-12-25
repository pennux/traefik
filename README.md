# Traefik
Repositório para colocar os arquivos que montei para usar o traefik como ingress controler, nesse momento o controle está somente na porta 80.

## Sequincia de intalação:

1 - Instalação do yaml para incluir a regras RBAC: <br > 
kubectl apply -f traefik-clusterrole.yaml

2 - Instalação do yaml para construir o container do tipo deamonset, que vai incluir um contariner em todo novo worker que subir:
kubectl apply -f traefik-deamonset.yaml

3 - Instalação do ymal para subir a interface de gerenciamento do traefik:
kubectl apply -f traefik-ui.yaml

[Documentação oficial](https://doc.traefik.io/traefik/ "Clique e acesse agora!")
