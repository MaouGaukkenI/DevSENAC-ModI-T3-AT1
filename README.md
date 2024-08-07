# Hospital Management System

## Description

This project is a hospital management system designed to facilitate the management of appointments, medical prescriptions, patients, doctors, and insurance providers. The database structure is designed to support common operations in a hospital environment, ensuring data integrity and efficient processing of information.

## Database Structure

The `hospital_db_Diogo` database consists of the following tables:

### 1. Patients
Stores information about the hospital's patients, including personal and contact details.

- **id**: Unique identifier for the patient.
- **name**: Patient's name.
- **date_of_birth**: Patient's date of birth.
- **address**: Patient's address.
- **phone**: Patient's phone number.
- **email**: Patient's email address.
- **CPF**: Patient's CPF number.
- **RG**: Patient's RG number.

### 2. Doctors
Contains information about the doctors working at the hospital.

- **id**: Unique identifier for the doctor.
- **name**: Doctor's name.
- **date_of_birth**: Doctor's date of birth.
- **address**: Doctor's address.
- **phone**: Doctor's phone number.
- **email**: Doctor's email address.

### 3. Specializations
Records the medical specializations available at the hospital.

- **id**: Unique identifier for the specialization.
- **name**: Name of the specialization.

### 4. Doctor_specialization
Associates doctors with their specializations.

- **id**: Unique identifier for the association.
- **doctor_id**: Reference to the doctor.
- **specialization_id**: Reference to the specialization.

### 5. Insurance Providers
Stores information about the insurance providers accepted by the hospital.

- **id**: Unique identifier for the insurance provider.
- **name**: Name of the insurance provider.
- **CNPJ**: CNPJ of the insurance provider.

### 6. Grace Period
Tracks the grace period for patient insurance.

- **id**: Unique identifier for the record.
- **grace_period**: Date and time when the grace period starts.
- **insurance_id**: Reference to the insurance provider.
- **patient_id**: Reference to the patient.

### 7. Appointments
Stores information about appointments held at the hospital.

- **id**: Unique identifier for the appointment.
- **date_time**: Date and time of the appointment.
- **doctor_id**: Reference to the doctor.
- **patient_id**: Reference to the patient.
- **amount**: Amount charged for the appointment.
- **insurance_id**: Reference to the insurance provider (if applicable).
- **insurance_card_number**: Insurance card number (if applicable).
- **specialization_id**: Reference to the specialization of the appointment.

### 8. Prescriptions
Contains information about the medical prescriptions issued.

- **id**: Unique identifier for the prescription.
- **medication**: Name of the medication.
- **quantity**: Quantity of the medication.
- **usage_instructions**: Instructions for using the medication.
- **appointment_id**: Reference to the associated appointment.

## Conclusion

This system provides a robust structure for managing hospital information, making it easier to organize and access the necessary data for efficient hospital operation. It allows for the tracking of patients, appointments, prescriptions, and more, ensuring a more effective and organized management.

## How to Use

To use this system, you will need to set up the database according to the provided instructions and integrate the system with the application that will interact with the database. Make sure to review the structure and adapt the system to meet the specific needs of your hospital environment.


# Sistema de Gestão Hospitalar--Traduzido:

## Descrição

Este projeto é um sistema de gestão hospitalar desenvolvido para facilitar o gerenciamento de consultas, receitas médicas, pacientes, médicos e convênios. A estrutura do banco de dados é projetada para suportar operações comuns em um ambiente hospitalar, garantindo a integridade dos dados e a eficiência no processamento das informações.

## Estrutura do Banco de Dados

O banco de dados `hospital_db_Diogo` é composto pelas seguintes tabelas:

### 1. Pacientes
Armazena informações sobre os pacientes do hospital, incluindo dados pessoais e de contato.

- **id**: Identificador único do paciente.
- **nome**: Nome do paciente.
- **data_de_nascimento**: Data de nascimento do paciente.
- **endereco**: Endereço do paciente.
- **telefone**: Número de telefone do paciente.
- **e-mail**: Endereço de e-mail do paciente.
- **CPF**: Número do CPF do paciente.
- **RG**: Número do RG do paciente.

### 2. Médicos
Contém dados sobre os médicos que atuam no hospital.

- **id**: Identificador único do médico.
- **nome**: Nome do médico.
- **data_de_nascimento**: Data de nascimento do médico.
- **endereco**: Endereço do médico.
- **telefone**: Número de telefone do médico.
- **e-mail**: Endereço de e-mail do médico.

### 3. Especializações
Registra as especializações médicas disponíveis no hospital.

- **id**: Identificador único da especialização.
- **nome**: Nome da especialização.

### 4. Medico_especializacao
Associa médicos às suas especializações.

- **id**: Identificador único da associação.
- **medico_id**: Referência ao médico.
- **especializacao_id**: Referência à especialização.

### 5. Convênios
Armazena informações sobre os convênios aceitos pelo hospital.

- **id**: Identificador único do convênio.
- **nome**: Nome do convênio.
- **CNPJ**: CNPJ do convênio.

### 6. Tempo_de_carencia
Controla o tempo de carência para convênios de pacientes.

- **id**: Identificador único do registro.
- **Tempo_de_carencia**: Data e hora do início do tempo de carência.
- **convenio_id**: Referência ao convênio.
- **paciente_id**: Referência ao paciente.

### 7. Consulta
Armazena informações sobre consultas realizadas no hospital.

- **id**: Identificador único da consulta.
- **data_hora**: Data e hora da consulta.
- **medico_id**: Referência ao médico.
- **paciente_id**: Referência ao paciente.
- **valor**: Valor cobrado pela consulta.
- **convenio_id**: Referência ao convênio (se aplicável).
- **numero_carteira**: Número da carteira do convênio (se aplicável).
- **especialidade_id**: Referência à especialização da consulta.

### 8. Receitas
Contém informações sobre as receitas médicas emitidas.

- **id**: Identificador único da receita.
- **medicamento**: Nome do medicamento.
- **quantidade**: Quantidade do medicamento.
- **instrucoes_de_uso**: Instruções de uso do medicamento.
- **consulta_id**: Referência à consulta associada à receita.

## Conclusão

Este sistema fornece uma estrutura robusta para gerenciar informações hospitalares, facilitando a organização e o acesso aos dados necessários para o funcionamento eficiente de um hospital. Com ele, é possível realizar o acompanhamento de pacientes, consultas, receitas e muito mais, garantindo uma gestão mais eficaz e organizada.

## Como Usar

Para usar este sistema, você precisará configurar o banco de dados conforme as instruções fornecidas e integrar o sistema com a aplicação que irá interagir com o banco de dados. Certifique-se de revisar a estrutura e adaptar o sistema conforme as necessidades específicas do seu ambiente hospitalar.
