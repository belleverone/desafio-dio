# desafio-dio
Desafio Criando um Organizador de Declaração de Imposto de Renda
import pandas as pd

# Load the uploaded Excel file
file_path = "/mnt/data/PROJETO IMPOSTO DE RENDA.xlsx"
excel_file = pd.ExcelFile(file_path)

# List all sheet names
sheet_names = excel_file.sheet_names

# Load a preview of each sheet to understand their contents
sheet_previews = {sheet: excel_file.parse(sheet).head() for sheet in sheet_names}
sheet_names, sheet_previews
**Resultado
(['TITULAR', 'INFORMES', 'NOTAS', 'TABELAS'],
 {'TITULAR':    Unnamed: 0  Unnamed: 1                                     Unnamed: 2  \
  0         NaN         NaN                                            NaN   
  1         NaN         NaN                            1. DADOS DO TÍTULAR   
  2         NaN         NaN  preencha os dados da sua pessoa física abaixo   
  3         NaN         NaN                                            NaN   
  4         NaN         NaN                                           NOME   
  
                  Unnamed: 3  
  0                      NaN  
  1                      NaN  
  2                      NaN  
  3                      NaN  
  4  Maria Antonia de Fátima  ,
  'INFORMES':    Unnamed: 0  Unnamed: 1                                    Unnamed: 2  \
  0         NaN         NaN                                           NaN   
  1         NaN         NaN          2. INFORMES DE RENDIMENTOS BANCÁRIOS   
  2         NaN         NaN  Preencha com seus dados atuais de cada banco   
  3         NaN         NaN                                           NaN   
  4         NaN         NaN                                         TOTAL   
  
    Unnamed: 3  
  0        NaN  
  1        NaN  
  2        NaN  
  3        NaN  
  4        NaN  ,
  'NOTAS':    Unnamed: 0  Unnamed: 1                                         Unnamed: 2  \
  0         NaN         NaN                                                NaN   
  1         NaN         NaN         3. NOTAS BANCÁRIAS OU EXTRATO DE HOLERITES   
  2         NaN         NaN  São todos os valores de entrada mês a mês de r...   
  3         NaN         NaN                                                NaN   
  4         NaN         NaN                                                NaN   
  
    Unnamed: 3 Unnamed: 4  
  0        NaN        NaN  
  1        NaN        NaN  
  2        NaN        NaN  
  3        NaN        NaN  
  4        NaN        NaN  ,
  'TABELAS':                                 bancos
  0                  1 - Banco do Brasil
  1    102 - XP Investimentos CCTVM S.A.
  2        104 - Caixa Econômica Federal
  3  119 - Banco Western Union do Brasil
  4            184 - Banco Itaú BBA S.A.})
Segue um modelo de arquivo README.md para o Excel intitulado "PROJETO IMPOSTO DE RENDA.xlsx". Este arquivo serve como guia de preenchimento e organização de dados para a declaração do Imposto de Renda de uma pessoa física.

PROJETO IMPOSTO DE RENDA
Este projeto tem como objetivo organizar e facilitar o preenchimento da declaração anual de Imposto de Renda para pessoas físicas no Brasil. O arquivo contém quatro planilhas com instruções e campos para preenchimento manual.

Estrutura do Arquivo
1. TITULAR
Contém os dados cadastrais da pessoa que está realizando a declaração:

Nome completo

CPF

Data de nascimento

Endereço

Dependentes (caso haja)

⚠️ Instruções: Preencher todos os dados pessoais conforme documentos oficiais.

2. INFORMES
Destinada à inserção dos informes de rendimentos bancários recebidos das instituições financeiras.

Instituição bancária

Valores recebidos

Tipo de rendimento (ex.: poupança, CDB, fundos)

⚠️ Instruções: Utilize os informes oficiais disponibilizados pelos bancos.

3. NOTAS
Planilha para registro mensal dos valores recebidos por meio de extratos bancários, contracheques (holerites), ou comprovantes de pagamentos.

Entradas financeiras mês a mês

Fonte pagadora

Observações relevantes (13º salário, férias, etc.)

⚠️ Instruções: Organize mês a mês os valores brutos recebidos.

4. TABELAS
Tabela de referência com os códigos e nomes dos bancos, que pode ser usada nas planilhas anteriores para padronização de dados.

🏦 Exemplo:

1 - Banco do Brasil

104 - Caixa Econômica Federal

119 - Banco Western Union do Brasil

Instruções Gerais
Todas as planilhas contêm instruções no topo.

Recomenda-se seguir a ordem: preencher primeiro a planilha TITULAR, depois INFORMES, seguida de NOTAS.

A planilha TABELAS é apenas para consulta.

Finalidade
Este projeto auxilia na organização prévia dos dados para posterior inserção no sistema da Receita Federal, tornando o processo de declaração mais simples, seguro e organizado.

**
