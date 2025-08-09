# Documento de Requisitos

## 1. Objetivo

Permitir o agendamento e cancelamento de consultas sem conflito de horários, bem como permitir que o médico cadastre sua disponibilidade.

---

## 2. Escopo

### Escopo **IN** (Incluso)
- Cadastro de usuários  
- Cadastro de pacientes  
- Cadastro da disponibilidade de cada médico  
- Agendamento e cancelamento de consultas  
- Exibição de mensagem de erro em caso de conflito de horário  

### Escopo **OUT** (Fora do escopo)
- Agendamento online (via site ou aplicativo externo)  
- Envio de mensagens para médicos  
- Faturamento e cobrança  
- Relatórios avançados  
- Histórico de consultas dos pacientes  

---

## 3. Regras de Negócio

- A clínica pode ter até **10 profissionais**.  
- Caso a consulta seja cancelada, o horário deverá ser liberado imediatamente.  
- A duração máxima de uma consulta é de **30 minutos**.  
- Não pode haver **sobreposição de horários** entre consultas.  
- Não pode haver **conflito de horário** entre agendamentos.

---

## 4. Premissas

- A clínica funcionará das **08h00 às 18h00**.  
- O banco de dados inicial terá no máximo **500 pacientes**.  
- Este é um **MVP (Produto Mínimo Viável)** com limitações.  
- Perfis de acesso contemplados:
  - Atendentes  
  - Médicos  
  - Pacientes  
  - Gestor da clínica  