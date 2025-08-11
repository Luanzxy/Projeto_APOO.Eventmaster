# Projeto A.P.O.O - Eventmaster

Documentação do projeto desenvolvido como atividade da disciplina de Análise e Projeto Orientado a Objetos (A.P.O.O).

---

## Visão do Produto

### Objetivo

O sistema tem como objetivo facilitar o gerenciamento de eventos educacionais e culturais, automatizando processos como cadastro de eventos, inscrições de participantes, gestão de palestrantes e emissão de certificados digitais.

### Público-alvo

* Instituições de ensino
* Organizações que promovem eventos, cursos e palestras
* Participantes de eventos

### Principais funcionalidades

* Cadastro de eventos (nome, data, local, descrição, capacidade)
* Cadastro de participantes
* Controle de inscrições nos eventos
* Cadastro e gerenciamento de palestrantes
* Emissão de certificados digitais
* Envio de notificações por e-mail
* Geração de relatórios de presença e inscritos

### Restrições e Premissas

* Aplicação web responsiva
* Envio de e-mails automático
* Geração de certificados com link único
* Sistema baseado no estudo de caso da disciplina de banco de dados

---

## Casos de uso

Descrição dos principais casos de uso do sistema:

### Caso de uso 1: Login

* **Atores:** Usuários autorizados (admin, organizador)
* **Fluxo principal:**

  1. Usuário acessa o sistema
  2. Informa login e senha
  3. Sistema valida e concede acesso

### Caso de uso 2: Cadastrar Evento

* **Atores:** Organizador
* **Fluxo principal:**
  1. Acessa área de eventos
  2. Insere nome, descrição, data, local e capacidade
  3. Sistema salva o novo evento

### Caso de uso 3: Inscrever Participante

* **Atores:** Participante
* **Fluxo principal:**
  1. Acessa página do evento
  2. Preenche dados e confirma inscrição
  3. Sistema registra a inscrição

### Caso de uso 4: Emitir Certificados

* **Atores:** Organizador
* **Fluxo principal:**

  1. Após o evento, acessa área de certificados
  2. Seleciona participantes presentes
  3. Sistema gera certificados e envia por e-mail

Para os diagramas, veja o arquivo `diagrama-casos-de-uso.png`.

---

## Modelo conceitual

O modelo conceitual descreve as entidades e relações principais do sistema.

### Entidades principais:

* **Evento:** id\_evento, nome, descrição, data_local, capacidade
* **Participante:** cpf, nome, email
* **Inscrição:** id\_inscricao, data\_inscricao, presença
* **Palestrante:** cpf, nome, email, mini\_curriculo
* **Certificado:** id\_certificado, data\_emissao, link\_certificado
* **Notificação:** id\_notificacao, tipo, data\_envio


Ver imagem `modelo-conceitual.png` e arquivo `modelo-conceitual.md` para detalhes e descrição textual das classes.

---

## Tecnologias utilizadas

* Github Codespaces para a escrita da documentação em Markdown
* Diagramas elaborados com Astah e Lucidchart
* Repositório hospedado no GitHub

---

## Equipe

| Nome                                     | Matrícula      |
| ---------------------------------------- | -------------- |
| José Luan Ribeiro Vieira                 | 20241011110023 |
| Lucas Gabriel da Silva Duarte            | 20241011110026 |
| Winnicius da Silva Faustino de Alcântara | 20241011110032 |
