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

