# Iniciar o projeto

    docker compose up



# Atualizar/Recriar imagem do container

    docker compose up --build


# Serviços disponíveis

    docker compose up n8n
    docker compose up mysql
    docker compose up redis
    docker compose up evolution-api



# Instalar os Nodes da Evolution API se não tiver:

    No N8N, vá em "Settings" → "Community Nodes" → "Install a community node" e digite: 
    n8n-nodes-evolution-api
    n8n-nodes-convert-image


# Executar workflow: Conectar Número Whatsapp no Evolution API Docker

    Exemplo:
    http://localhost:5678/webhook/qrcode?instance=INSTANCE_NAME&number=5532991919191

# Limpar projeto

    docker compose down
    docker volume ls
    docker volume rm n8n_mysql_data
    docker volume rm n8n_n8n_data
    docker volume rm n8n_redis_data
