# Minha Primeira Stack com AWS CloudFormation

## 📝 Introdução
Este projeto foi desenvolvido como parte do desafio da DIO, com o objetivo de criar minha primeira **Stack na AWS utilizando CloudFormation**.  
A Stack inclui recursos básicos para prática e aprendizado, permitindo compreender a estrutura, deployment e monitoramento de recursos AWS.

---

## 📦 Recursos Criados
| Recurso        | Tipo AWS               | Descrição                                    |
|----------------|----------------------|---------------------------------------------|
| MinhaInstanciaEC2 | AWS::EC2::Instance   | Instância EC2 para testes                    |
| MeuBucketS3    | AWS::S3::Bucket       | Bucket S3 para armazenamento de arquivos    |

**Outputs:**  
- `EC2InstanceID` → ID da instância EC2 criada  
- `S3BucketName` → Nome do bucket S3 criado

---

## ⚙️ Estrutura do Projeto


---

## 🚀 Instruções para Executar a Stack
1. Acesse o console da AWS CloudFormation.  
2. Clique em **Criar Stack** → **Com recursos novos** → **Enviar template**.  
3. Faça upload do arquivo `template.yaml`.  
4. Preencha os parâmetros (ex.: tipo de instância EC2).  
5. Clique em **Próximo** e depois em **Criar Stack**.  
6. Aguarde a criação dos recursos e confira os outputs.

---

## 📸 Capturas de Tela
> Substitua as imagens pelos prints da sua execução no console.

![CloudFormation Stack](images/stack_creation.png)  
*Exemplo de Stack sendo criada*

![Outputs](images/stack_outputs.png)  
*Exemplo de outputs gerados*

---

## 💡 Aprendizados e Insights
- Aprendi a estruturar um template CloudFormation em **YAML**.  
- Testei parâmetros para tornar a Stack mais flexível.  
- Entendi como usar **outputs** para consultar recursos criados.  
- Capturei erros comuns e como corrigi-los (ex.: conflitos de nomes de recursos).  

---

## 🔗 Referências
- [AWS CloudFormation Documentation](https://docs.aws.amazon.com/cloudformation/index.html)  
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)  

---

> Autor: Bianca
> Data: 31/10/2025

# 🚀 Gerenciando Recursos na AWS: EC2, S3 e Lambda  

Este projeto tem como objetivo **entender e aplicar os principais serviços de computação, armazenamento e execução serverless da AWS** — o **Amazon EC2**, **Amazon S3** e **AWS Lambda** — mostrando como eles se conectam entre si para formar soluções modernas em nuvem.  

---

## 💻 **Amazon EC2 — Servidores (Máquinas Virtuais)**  

**O que é:**  
O **Amazon EC2 (Elastic Compute Cloud)** é o serviço de **computação em nuvem** da AWS.  
Com ele, é possível **alugar máquinas virtuais (instâncias)** sob demanda, escolhendo o tamanho, o sistema operacional e os recursos necessários (CPU, RAM, rede, etc.).  

**Exemplo simples:**  
> Você aluga um computador na nuvem, instala o que quiser e o usa como servidor.  

**Casos de uso:**  
- Hospedar um site ou sistema web  
- Executar um servidor de jogos  
- Rodar aplicações corporativas  

---

## 📦 **Amazon S3 — Armazenamento de Objetos**  

**O que é:**  
O **Amazon S3 (Simple Storage Service)** é o serviço de **armazenamento de objetos** da AWS.  
Funciona como um **cofre infinito** para guardar qualquer tipo de arquivo (imagens, vídeos, backups, logs) de forma segura, durável e escalável.  

**Exemplo simples:**  
> Guardar todas as imagens do seu aplicativo de forma segura e acessível.  

**Casos de uso:**  
- Armazenar arquivos, logs e backups  
- Hospedar sites estáticos  
- Armazenar dados para machine learning ou big data  

---

## ⚙️ **AWS Lambda — Computação Sem Servidor (Serverless)**  

**O que é:**  
O **AWS Lambda** é um serviço **serverless**, ou seja, **executa código sob demanda sem precisar configurar ou gerenciar servidores**.  
Você escreve apenas o código, define o evento que o dispara (trigger), e a AWS cuida do resto.  

**Exemplo simples:**  
> Processar automaticamente uma imagem assim que ela é salva no S3.  

**Casos de uso:**  
- Automatizar tarefas (como processamento de imagens)  
- Criar backends de APIs sem servidor  
- Integrar com eventos de outros serviços da AWS (como S3, DynamoDB, SNS, etc.)  

---

## 🔗 **Como Eles se Conectam**  

Esses serviços **trabalham juntos** de forma integrada, permitindo construir soluções completas em nuvem:  

| Integração | Descrição |
|-------------|------------|
| **EC2 → S3** | Uma instância EC2 pode salvar e ler arquivos diretamente de um bucket S3. |
| **S3 → Lambda** | O upload de um arquivo no S3 pode **disparar uma função Lambda** automaticamente. |
| **Lambda → EC2 / S3** | Uma função Lambda pode processar dados do S3 ou acionar uma instância EC2 conforme necessário. |

**Fluxo prático de exemplo:**  
1. Um usuário faz upload de uma imagem no **S3**.  
2. O evento aciona uma **função Lambda** que processa a imagem (ex: redimensiona).  
3. A função salva o resultado novamente no **S3**.  
4. Uma instância **EC2** pode usar a imagem processada em um site hospedado.  

---

## 🧩 **Resumo Final**

| Serviço | Tipo | O que faz | Exemplo prático |
|----------|------|------------|----------------|
| **Amazon EC2** | Computação | Executa servidores e aplicações | Hospedar um site |
| **Amazon S3** | Armazenamento | Guarda arquivos e dados | Armazenar imagens |
| **AWS Lambda** | Serverless | Executa código sob demanda | Processar uma imagem automaticamente |

---

## 🛠️ **Ferramentas utilizadas**
- AWS Management Console  
- Amazon EC2  
- Amazon S3  
- AWS Lambda  
- IAM (para permissões e roles)  

---

## 🌟 **Aprendizados**
- Entendimento sobre a diferença entre **computação tradicional (EC2)** e **serverless (Lambda)**.  
- Como o **S3** atua como o principal serviço de **armazenamento de objetos** na nuvem AWS.  
- Integração entre serviços para criar fluxos automatizados e escaláveis.  

---

📘 **Autora:** [Bianca Queiroz](https://github.com/)  
💡 **Desafio:** *Criando Recursos na AWS — EC2, S3 e Lambda*  
📅 **Plataforma:** [Digital Innovation One (DIO)](https://www.dio.me/)

---
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/9383cfde-7faf-4bd4-a898-d3316e45cbc8" />
