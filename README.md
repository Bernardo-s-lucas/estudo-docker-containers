# Estudo Docker - Containers

## Sobre
Este repositório documenta meu aprendizado sobre Docker e containerização.

**Autor:** Bernardo Silva
**Curso:** Segurança Cibernética
**Disciplina:** Banco de Dados
**Data:** 09/09/2026

## O que estou aprendendo
- Conceitos fundamentais do Docker
- Como criar e gerenciar containers
- Trabalhar com imagens Docker
- Configurar bancos de dados em containers
- Usar Docker Compose para aplicações multi-container

## Estrutura do Projeto
- `containers/` - Dockerfiles e configurações de containers
- `compose/` - Arquivos docker-compose.yml
- `scripts/` - Scripts de configuração e inicialização
- `README.md` - Este arquivo de documentação

## Status do Estudo
- [✅] Tarefa 1 - Primeiro container
- [✅] Tarefa 2 - Container personalizado
- [✅] Tarefa 3 - Banco de dados
- [✅] Tarefa 4 - Docker Compose
- [✅] Tarefa 5 - Aplicação completa

## 🧐 Reflexão Final

**1.Qual a principal vantagem de usar containers com Docker em vez de instalar um banco de dados e um servidor web diretamente na sua máquina?**

O Docker isola os serviços em containers leves, evitando poluir o sistema operacional com instalações diretas (como MySQL ou Python) e eliminando conflitos de versões.

**2.Explique com suas palavras o propósito de um Dockerfile. Por que ele é tão importante para a reprodutibilidade de ambientes?**

É o script com a "receita" para criar uma imagem. Ele garante que qualquer pessoa consiga rodar exatamente a mesma aplicação em qualquer computador sem erros de ambiente.

**3.Em que cenário o Docker Compose se torna essencial? Por que não usar apenas múltiplos comandos docker run?**

O Compose orquestra múltiplos containers (ex: Web + Banco) em um único arquivo `docker-compose.yml`, evitando ter que rodar vários comandos `docker run` manuais para configurar redes e portas.

**4.Qual a importância dos volumes do Docker (como o que usamos para o banco de dados MySQL)? O que aconteceria com os dados se não usássemos um volume?**

Garantem a **persistência dos dados**. Como o container é descartável, sem o volume todos os dados do banco MySQL seriam apagados quando o container fosse parado.

**5.Como o uso de containers pode facilitar o trabalho em equipe em um projeto de desenvolvimento de software?**

Padroniza o ambiente para todo mundo do time. Qualquer dev pode clonar o projeto e rodar a aplicação idêntica em segundos.