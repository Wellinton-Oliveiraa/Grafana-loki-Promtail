# Criar uma rede (com nome de loki no servidor sidecar)
docker network create loki

# Verificar a questão de permissões na pasta /loki/wal/

# Para coletar logs de Containers em outro servidor alterar o localhost pelo ip do loki na configuração do promtail:
clients:
  - url: http://localhost:3100/loki/api/v1/push
