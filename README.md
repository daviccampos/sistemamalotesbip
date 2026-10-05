# Sistema de Controlo e Automação de Malotes (BIP)

Sistema de automação logística desenvolvido em Python com o objetivo de otimizar e agilizar o registo, o rastreio, a conferência e a geração de protocolos de malotes postais. A aplicação foi concebida para transformar um processo manual, sujeito a falhas humanas, num fluxo integrado e automatizado através da leitura de códigos de barras[cite: 2].

---

## Tecnologias Utilizadas

O projeto foi estruturado com base nos fundamentos de Análise e Desenvolvimento de Sistemas, utilizando as seguintes tecnologias e bibliotecas:
* Python 3.x (Linguagem de programação principal)
* FreeSimpleGUI (Interface gráfica de utilizador organizada por abas operacionais)[cite: 2]
* Pandas (Manipulação, tratamento e persistência de dados tabulares)[cite: 2]
* OpenPyXL (Estilização avançada e automação de planilhas em formato Excel)[cite: 2]
* CSV, OS e Time (Gestão de diretórios locais, ficheiros de configuração e eventos de periféricos)[cite: 2]

---

## Funcionalidades Principais

1. **Leitura Automatizada por Código de Barras:** Captura automática de códigos padronizados com 35 dígitos, extraindo de forma instantânea o posto e o número sequencial do malote, eliminando a digitação manual[cite: 2].
2. **Mapeamento Dinâmico de Postos:** Mecanismo de associação e registo de novos códigos através de um ficheiro de configuração persistente (`postos_codigos.csv`), assegurando a integridade dos dados operacionais[cite: 2].
3. **Gestão Operacional por Abas Diárias:** Interface dividida entre os dias da semana (Segunda a Sexta-feira), Capital e a secção de Recebidos[cite: 2].
4. **Controlo de Pendentes e Concluídos:** Atualização em tempo real das listas de postos restantes para envio e contagem total de registos[cite: 2].
5. **Geração Automatizada de Protocolos:** Emissão de manifestos de envio para o Interior e Capital (`PROTOCOLO INTERIOR` e `PROTOCOLO CAPITAL`), formatados com bordas, alinhamentos e totalizadores prontos para impressão[cite: 2].
6. **Persistência de Dados:** Armazenamento estruturado e centralizado em ambiente local num ficheiro Excel (`controle_malotes_v85.xlsx`)[cite: 2].

---

## Instruções de Execução

### Pré-requisitos
Certifique-se de que o Python está instalado no ambiente de execução. Instale as dependências necessárias através do terminal utilizando o comando seguinte:

```bash
pip install pandas FreeSimpleGUI openpyxl
