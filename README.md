<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=66CDAA&height=120&section=header"/>

# WEBSCRAPING

Projeto desenvolvido para o processo seletivo de Estágio em **Ciências de Dados**, utilizando a linguagem **Python** e os princípios fundamentais das bibliotecas **pandas, zipfile e BeautifulSoup.**.

---

## 🎯 Objetivos do Projeto

O objetivo é criar uma script simples (WEBSCRAPING) em Python que receba uma pasta compactada no formato .zip, contendo um conjunto de arquivos HTML. A aplicação deve descompactar o arquivo .zip e, para cada arquivo HTML processado, extrair uma tabela com as seguintes features (características):

*   Nome do Arquivo
*   CNPJ
*   RESULTADO

SE HOUVER RESULTADOS:

*   NÚMERO DO PEDIDO
*   DATA DO DEPÓSITO
*   TÍTULO
*   IPC
  
Por fim, foram gerado um Data Frame com as features.

---

## 👨‍💻 Características do Arquivo 
Arquivo no formato .zip contendo um conjunto de arquivos HTML, os quais possuem informações importantes para a extração e geração de features, utilizadas na criação da base de dados.

---

##  📋 Explicação sobre o projeto:

1. Extração dos arquivos HTML:
O script descompacta automaticamente o arquivo ZIP e armazena todos os arquivos HTML em uma nova pasta (“PATENTES”).

2. Leitura e detecção de encoding:
Cada arquivo HTML é aberto em modo binário, e o chardet é utilizado para identificar o tipo de codificação, garantindo que o conteúdo seja lido corretamente.

3. Análise e extração dos dados:
Utilizando o BeautifulSoup, o código percorre o conteúdo HTML e extrai informações específicas, como:

- CNPJ do depositante (ou CPF, quando aplicável);
- Número do pedido de patente;
- Data do depósito;
- Título do pedido;
- Código IPC;
- Quantidade de resultados encontrados por arquivo.

4. Tratamento de arquivos sem resultados:
Caso o arquivo HTML contenha um resultado igual a “0”, o script registra o arquivo com os campos nulos, mantendo a consistência dos dados.

5. Organização em DataFrame:
Todas as informações coletadas são armazenadas em uma lista de dicionários e, ao final, convertidas em um DataFrame do pandas, facilitando a análise, exportação e manipulação posterior.

---

## Equipe do Projeto

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="https://avatars.githubusercontent.com/u/155683708?v=4" width="100px" alt="Lucas Cabral"/><br/>
        <b>Lucas Cabral</b>
      </td>
    </tr>
  </table>
</div>

---

<p align="center">
  &copy; 2025 Universidade Federal de Pernambuco - Centro de Informática. Todos os direitos reservados.
</p>

<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=66CDAA&height=120&section=header"/>
