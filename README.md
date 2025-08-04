# Projeto A.P.O.O - Eventmaster

Documentação do projeto desenvolvido como atividade da disciplina de Análise e Projeto Orientado a Objetos (A.P.O.O).

---

## 📌 visão do produto

### 🎯 objetivo

O sistema tem como objetivo facilitar o gerenciamento de eventos educacionais e culturais, automatizando processos como cadastro de eventos, inscrições de participantes, gestão de palestrantes e emissão de certificados digitais.

### 👥 público-alvo

* instituições de ensino
* organizações que promovem eventos, cursos e palestras
* participantes de eventos

### ⚙️ principais funcionalidades

* cadastro de eventos (nome, data, local, descrição, capacidade)
* cadastro de participantes
* controle de inscrições nos eventos
* cadastro e gerenciamento de palestrantes
* emissão de certificados digitais
* envio de notificações por e-mail
* geração de relatórios de presença e inscritos

### 🔒 restrições e premissas

* aplicação web responsiva
* envio de e-mails automático
* geração de certificados com link único
* sistema baseado no estudo de caso da disciplina de banco de dados

---

## 📚 casos de uso

descrição dos principais casos de uso do sistema:

### caso de uso 1: login

* **atores:** usuários autorizados (admin, organizador)
* **fluxo principal:**

  1. usuário acessa o sistema
  2. informa login e senha
  3. sistema valida e concede acesso

### caso de uso 2: cadastrar evento

* **atores:** organizador
* **fluxo principal:**

  1. acessa área de eventos
  2. insere nome, descrição, data, local e capacidade
  3. sistema salva o novo evento

### caso de uso 3: inscrever participante

* **atores:** participante
* **fluxo principal:**

  1. acessa página do evento
  2. preenche dados e confirma inscrição
  3. sistema registra a inscrição

### caso de uso 4: emitir certificados

* **atores:** organizador
* **fluxo principal:**

  1. após o evento, acessa área de certificados
  2. seleciona participantes presentes
  3. sistema gera certificados e envia por e-mail

para os diagramas, veja o arquivo `casos-de-uso.md`.

---

## 🧠 modelo conceitual

o modelo conceitual descreve as entidades e relações principais do sistema.

### entidades principais:

* **evento:** id\_evento, nome, descrição, data, local, capacidade
* **participante:** cpf, nome, email
* **inscrição:** id\_inscricao, data\_inscricao, presença
* **palestrante:** cpf, nome, email, mini\_curriculo
* **certificado:** id\_certificado, data\_emissao, link\_certificado
* **notificação:** id\_notificacao, tipo, data\_envio

### relações:

* Um evento tem muitas inscrições
* Um participante pode ter muitas inscrições
* Uma inscrição pode gerar um certificado
* Notificações são enviadas para participantes e eventos
* Eventos possuem palestrantes (relação n para n)

ver imagem `modelo-conceitual.png` e arquivo `modelo-conceitual.md` para detalhes e descrição textual das classes.

---

## 🛠️ tecnologias utilizadas

* Github Codespaces para documentação com Markdown
* Astah para diagramas
* Github para fasdasdasdasd do repositório

---

## 👨‍💻 equipe

| Nome                                     | Matrícula      |
| ---------------------------------------- | -------------- |
| José Luan Ribeiro Vieira                 | 20241011110023 |
| Lucas Gabriel da Silva Duarte            | 20241011110026 |
| Winnicius da Silva Faustino de Alcântara | 20241011110032 |
