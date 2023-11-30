##                                      <h1 align="center"> PetShop </h1>

**_PetShop_** é um aplicativo lowcode desenvolvido com  _Power Apps_ e destina-se ao gerenciamento de clínicas veterinárias. Por meio dele é possivel realizar o cadastro de clientes / animais e realizar o agendamento de serviços.


## Autora:
- Bruna Pacheco

## Desenvolvido com:

 - PowerApps
 - Power Automate
 - Figma

## Exemplo de uso:
(Canvas app - aplicativo de Tela)
1. Tela inicial - Acesso pelo botão Entrar;

2. Tela Cadastro do Cliente: preencher as informações do cliente;

3. Tela Cadastro do Animal: preencher informações sobre o animal que será atendido;
   
4. Tela de Agendamentos: agendamento do tipo de serviço, data e horário;
   
5. Tela de Confirmação: confirma que o agendamento foi realizado com sucesso e retorna a tela inicial.

![telaInicial](https://github.com/Bruna-Tec/PetShop/assets/150478974/ed60ae8a-41a7-4ead-8a6c-82766f783f1d)
![cadastroCliente](https://github.com/Bruna-Tec/PetShop/assets/150478974/18f4c7e0-a11c-40c0-bb92-1a1043a15eb1)
![cadastroAnimal](https://github.com/Bruna-Tec/PetShop/assets/150478974/291512a0-83a6-42a4-906b-79aef6121fd8)
![telaAgendamentos](https://github.com/Bruna-Tec/PetShop/assets/150478974/7af5359f-3cc9-455c-a8f1-bdfb6eff9d66)
![SucessoAgendamento](https://github.com/Bruna-Tec/PetShop/assets/150478974/bd9e30ad-1b75-4918-b303-1f67a1f01f81)

(Dataverse - armazenamento e modelagem de dados)

1. Tabela Cliente
   Atributos:
   - Nome
   - RG
   - CPF
   - Data Nascimento
   - Celular
   - E-mail
   - Endereço (Rua / N / Bairro / Cidade / Estado / CEP /  Complemento
   - Pendências
 2. Tabela Animal
    Atributos:
    - Nome do tutor (faz referência a nome do cliente)
    - Espécie
    - Raça
    - Nome do animal
    - Idade
    - Sexo (macho/fêmea)
    - Porte (pequeno / médio / grande)
    - Manso (sim / não)
    - Cor
    - Possui Doença (sim/não)
    - Descrição da Doença
  3. Agendamentos
     Atributos:
     - Tipo de Serviço (banho / tosa / banho e tosa / consulta / todos os serviços)
     - Animal (faz referência ao nome do animal)
     - Cliente (referência ao cliente)
     - Horário do início do agendamento (data e hora)
     - Horário do fim do agendamento (data e hora)
     - Valor do serviço
    
   (Power Automate - fluxos automatizados)
   1. Fluxo para consultar CEP
      
- Inicializando o fluxo e fazendo a requisição para API de CEP:
  
![fluxo2](https://github.com/Bruna-Tec/PetShop/assets/150478974/60352583-6b9d-45dc-87a6-13bfc7e344a6)

- Gerando dados usando modelo JSON e definindo as entradas:
  
![fluxo3](https://github.com/Bruna-Tec/PetShop/assets/150478974/2b783b91-09ba-433d-894a-c7f50a212734)

- Criando as variáveis:
  
![fluxo4](https://github.com/Bruna-Tec/PetShop/assets/150478974/d0076497-4186-4b2f-8814-0c834fb085e1)

- Definindo as variáveis:
  
![fluxo5](https://github.com/Bruna-Tec/PetShop/assets/150478974/ae0d4714-c5fe-4835-80bd-8863b4441351)

- Respondendo ao fluxo no power apps:
  
![fluxo6](https://github.com/Bruna-Tec/PetShop/assets/150478974/bc3350f6-9f00-4d38-936d-7d40a52bb965)


 
