# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS  

**Data:** 01/09/2025  
**Empresa:** Abstergo Industries  
**Responsável:** Gabriel Barbosa  

---

## Apresentação da empresa  
A Abstergo Industries é uma organização do setor farmacêutico que está expandindo sua atuação para se consolidar como um hub estratégico de distribuição de medicamentos. Com foco em eficiência logística e confiabilidade, a empresa estabelecerá parcerias sólidas com diversas companhias do segmento. Seu compromisso é garantir agilidade, segurança e qualidade no atendimento à cadeia de suprimentos farmacêutica.  

---

## Introdução  
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Gabriel Barbosa. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos, garantir escalabilidade e segurança.  

---

## Descrição do Projeto  

### Etapa 1  
- **Ferramenta:** Amazon S3 (Simple Storage Service)  
- **Foco da ferramenta:** Armazenamento seguro e escalável de dados.  
- **Descrição de caso de uso:** O S3 será usado para guardar documentos relacionados a medicamentos (notas fiscais, relatórios de controle, prescrições digitalizadas) e também para armazenar backups do sistema de gestão.  
- **O porquê desta ferramenta nesta etapa:** O S3 é simples de configurar e já garante um local seguro para guardar dados, backups e documentos da empresa antes mesmo de subir os sistemas, cobra apenas pelo que usar e elimina a necessidade de servidores físicos caros para guardar arquivos. Região de referência será **US East (N. Virginia – us-east-1)** para manter custos baixos.  

### Etapa 2  
- **Ferramenta:** Amazon RDS (Relational Database Service)  
- **Foco da ferramenta:** Banco de dados gerenciado.  
- **Descrição de caso de uso:** O RDS permitirá criar um banco de dados (como MySQL ou PostgreSQL) já configurado e seguro, para controlar estoque, pedidos e fornecedores. Sem que a equipe precise gerenciar hardware ou manutenção complexa. Isso reduz custos de administração de TI e garante alta disponibilidade para os sistemas de logística da empresa.  
- **O porquê desta ferramenta nesta etapa:** O banco precisa estar pronto antes do sistema rodar na EC2, já que o sistema vai se conectar a ele.  

### Etapa 3  
- **Ferramenta:** Amazon EC2 (Elastic Compute Cloud)  
- **Foco da ferramenta:** Servidores virtuais escaláveis.  
- **Descrição de caso de uso:** Para rodar o sistema principal da empresa (ex: ERP, sistema de controle de entregas e logística), a farmacêutica pode usar o EC2. Ele permite “ligar” e “desligar” servidores virtuais conforme a demanda.  
- **O porquê desta ferramenta nesta etapa:** O EC2 precisa consumir tanto o banco (RDS) quanto os arquivos (S3). Paga apenas pelo tempo em que a máquina estiver ativa, assim, não há gastos fixos com servidores físicos.  

---

## Conclusão  
A implementação de ferramentas na empresa Abstergo Industries tem como resultado esperado o aumento da eficiência operacional, a redução de custos e maior segurança no gerenciamento de dados, contribuindo para maior eficiência e produtividade organizacional. Recomenda-se a continuidade do uso das ferramentas implementadas e a busca constante por novas tecnologias em nuvem e soluções de automação que agreguem va


## Anexos  
- [Amazon EC2](https://aws.amazon.com/pt/ec2/?did=ft_card2&trk=ft_ec2)  
- [Amazon S3](https://aws.amazon.com/pt/s3/?did=ft_card2&trk=ft_s3)  
- [Amazon RDS](https://aws.amazon.com/pt/rds/?did=ft_card2&trk=ft_rds)  

---

**Assinatura do Responsável pelo Projeto:**  
Gabriel Barbosa  
