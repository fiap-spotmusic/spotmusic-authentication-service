# SpotMusic Payment Service

`spotmusic-payment-service`: Um microserviço seguro e escalável dedicado ao processamento de transações financeiras, permitindo aos usuários da SpotMusic realizar pagamentos de assinaturas e compras dentro do aplicativo

## Pilha Tecnológica
- **Linguagem de Programação:** Python com Flask
- **Banco de Dados:** PostgreSQL no Amazon RDS
- **Autenticação:** OAuth 2.0 / JWT Tokens
- **Monitoramento:** Zabbix

## Configuração e Instalação
Para configurar e executar o `spotmusic-payment-service` em seu ambiente de desenvolvimento, siga os passos abaixo:

```bash
# Clone o repositório
git clone https://github.com/fiap-spotmusic/spotmusic-payment-service.git
cd spotmusic-payment-service

# Instale as dependências
pip install -r requirements.txt

# Configure o arquivo .env com as variáveis de ambiente necessárias
cp .env.example .env
# Edite o arquivo .env com as configurações do seu ambiente
nano .env

# Carregue as variáveis de ambiente
source .env

# Execute as migrações para o banco de dados
flask db upgrade

# Inicie o serviço
flask run
