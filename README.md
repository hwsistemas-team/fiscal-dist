# fiscal-dist

Arquivos fiscais brutos para uso do ERP

## Arquivo: `calculadora.db`

Banco de dados SQLite extraido do container java da Calculadora de imposto da RTC

Nenhum tratamento necessário nos dados do arquivo
> Fonte: https://piloto-cbs.tributos.gov.br/servico/calculadora-consumo/calculadora/calculadora-offline

## Arquivo: `ibpt-??.csv`

Arquivo CSV com aliquotas aproximadas dos tributos que devem ser destacadas em todos os documentos fiscais destinados a consumidor final.

Nenhum tratamento necessário nos dados do arquivo
> Fonte: https://deolhonoimposto.ibpt.org.br/Empresa

* A fonte disponibiliza os dado por estado
* A fonte exige cadastro da empresa para fazer o dwonload
* O arquivo precisa ter os caracteres de `??` substituídos pela sigla da **UF**

## Arquivos: `ncm-historica.json`  `ncm-futura.json` e `ncm-vigentes.json`

Arquivos json com alista de NCM's históricos, futuros e vigentes

Nenhum tratamento necessário nos dados dos arquivos
> Fonte: https://portalunico.siscomex.gov.br/classif/#/nomenclatura/tabela?perfil=publico

* A fonte fornece o download dos 3 arquivos separados
* A fonte tem a validação do captcha no endereço

## Arquivo: `correl-fiscal-nfse.csv`

Arquivo que tem a correlação entre os códigos fiscais: Código do serviço da Lei Complementar `116` x `NBS` x `cIndOp` da NFSe no Padrao Nacional x `cClassTrib` do IBSCBS

###  O arquivo original é fornecido em `.xlsx` e foi convertido para `.csv`

* Utilizando o Excel para abrir o arquivo original e usar a opção de Exportar ou Salvar como.
* Escolha do formato: (CSV separado por vírgulas) (*csv)

> Fonte: https://www.gov.br/nfse/pt-br/biblioteca/documentacao-tecnica/documentacao-atual<br>
> Na lista de arquivos, seção **Anexos de Domínio**: `ANEXO_C-INDOP_IBSCBS-SNNFSe-v?.??-????????.xlsx`