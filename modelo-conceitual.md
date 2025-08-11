# modelo conceitual

o modelo conceitual representa as entidades e os relacionamentos principais do sistema eventmaster.

## Entidades:

### Evento

* id\_evento
* nome
* descricao
* data
* local
* capacidade

### Participante

* cpf
* nome
* email

### Inscricao

* id\_inscricao
* data\_inscricao
* presenca

### Palestrante

* cpf
* nome
* email
* mini\_curriculo

### Certificado

* id\_certificado
* data\_emissao
* link\_certificado

### Notificacao

* id\_notificacao
* tipo
* data\_envio

## Relacionamentos:

* **Evento \[1] ↔ \[0..n] Inscricao** → um evento tem várias inscrições
* **Participante \[1] ↔ \[0..n] Inscricao** → um participante pode se inscrever em vários eventos
* **Inscricao \[1] → \[0..1] Certificado** → uma inscrição pode gerar um certificado
* **Participante \[1] ↔ \[0..n] Notificacao** → participante recebe notificações
* **Evento \[1] ↔ \[0..n] Notificacao** → evento pode gerar notificações
* **Evento \[1] ↔ \[0..n] Palestrante** / **palestrante \[1] ↔ \[0..n] evento** → palestrantes participam de eventos (relação n\:n)
