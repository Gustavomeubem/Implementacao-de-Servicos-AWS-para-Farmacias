Projeto de Otimização de Custos AWS para Farmácias
📋 Descrição do Projeto
Este projeto implementa uma solução AWS para redução de custos em farmácias através de três serviços principais:

AWS Cost Explorer - Monitoramento e análise de custos

AWS Lambda - Automação de processos serverless

Amazon S3 Intelligent-Tiering - Armazenamento otimizado de dados

🎯 Objetivos
Reduzir custos de infraestrutura em 40% no primeiro ano

Automatizar processos manuais da farmácia

Otimizar armazenamento de documentos e dados

🛠️ Tecnologias Utilizadas
AWS Cost Explorer API - Para análise de custos

AWS Lambda - Para computação serverless

Amazon S3 - Para armazenamento inteligente

Boto3 - SDK Python para AWS

Python 3.9 - Linguagem de implementação

📊 Estrutura do Projeto
text
farmacia-cost-optimization/
│
├── cost_optimizer.py      # Classe principal de otimização
├── lambda_functions/      # Funções Lambda específicas
├── policies/             # Políticas IAM e S3
├── requirements.txt      # Dependências do projeto
└── README.md            # Documentação
⚙️ Configuração
Configure as credenciais AWS:

bash
aws configure
Instale as dependências:

bash
pip install -r requirements.txt
Execute o otimizador:

python
python cost_optimizer.py
🔐 Políticas IAM Necessárias
json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "ce:GetCostAndUsage",
                "lambda:CreateFunction",
                "s3:PutBucketIntelligentTieringConfiguration"
            ],
            "Resource": "*"
        }
    ]
}
📈 Métricas de Sucesso
Redução de 40% nos custos de EC2/RDS

Eliminação de 70% dos processos manuais

Economia de 60% em custos de armazenamento

🚀 Próximos Passos
Implementar AWS Budgets para alertas de custo

Adicionar Amazon QuickSight para dashboards

Integrar com sistema ERP da farmácia
