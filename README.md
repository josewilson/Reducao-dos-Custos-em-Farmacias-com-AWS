Relatório Técnico: Otimização de Custos na AWS para Farmácias
1. Introdução

A adoção de serviços em nuvem pela farmácia trouxe benefícios como escalabilidade e flexibilidade. No entanto, é essencial monitorar e otimizar os custos para garantir a sustentabilidade financeira da operação.

2. Cenário Atual

Serviços Utilizados: EC2, RDS, S3, Lambda.

Desafios Identificados:

Provisionamento excessivo de recursos.

Armazenamento de dados não estruturados em classes de armazenamento inadequadas.

Ausência de políticas de escalabilidade automática.

Falta de monitoramento contínuo de custos.

3. Estratégias de Otimização
3.1. Monitoramento e Análise de Custos

AWS Cost Explorer: Ferramenta para visualizar e analisar os custos e o uso dos serviços AWS. Permite identificar padrões de gasto e áreas de otimização.

AWS Budgets: Estabelece orçamentos personalizados e envia alertas quando os limites são atingidos.

AWS Cost Anomaly Detection: Detecta variações inesperadas nos custos, ajudando a identificar gastos não planejados.

3.2. Otimização de Recursos

Direcionamento de Instâncias EC2: Utilize instâncias Spot para cargas de trabalho tolerantes a falhas e instâncias reservadas para cargas previsíveis.

Escalabilidade Automática: Implemente Auto Scaling para ajustar automaticamente a capacidade de recursos com base na demanda.

Utilização de Graviton: Migrar para instâncias baseadas em Graviton pode reduzir custos em até 40% para cargas de trabalho compatíveis.

3.3. Armazenamento Eficiente

S3 Intelligent-Tiering: Move dados automaticamente entre duas classes de armazenamento quando há mudanças no acesso.

Amazon EBS: Utilize volumes com otimização de custo, como st1 ou sc1, para dados acessados com menos frequência.

3.4. Planejamento de Capacidade

AWS Compute Optimizer: Fornece recomendações para ajustar o tipo e o tamanho das instâncias EC2, RDS e EBS com base no uso real.

AWS Trusted Advisor: Oferece recomendações para melhorar a segurança, desempenho e reduzir custos.

4. Implementação Prática
4.1. Scripts e Templates

CloudFormation: Utilize templates para provisionar recursos de forma consistente e automatizada.

AWS Lambda: Automatize tarefas de manutenção e monitoramento com funções serverless.

4.2. Exemplos de Comandos
# Listar instâncias EC2
aws ec2 describe-instances

# Verificar volumes EBS
aws ec2 describe-volumes

# Obter recomendações do Compute Optimizer
aws compute-optimizer describe-recommendations

4.3. Monitoramento Contínuo

Amazon CloudWatch: Configure métricas e alarmes para monitorar o desempenho e os custos em tempo real.

AWS Cost and Usage Report (CUR): Gere relatórios detalhados para análise aprofundada.

5. Conclusão

Implementar as estratégias acima permitirá à farmácia reduzir significativamente seus custos operacionais na AWS, mantendo a performance e a escalabilidade necessárias para o crescimento do negócio.
