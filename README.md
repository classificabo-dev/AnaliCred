# AnaliCred
Este projeto realiza uma análise de crédito automatizada  de CNPJ, utilizando diversos indicadores financeiros
# Análise de Crédito 

Análise automatizada de crédito para empresas listadas , com geração de ratings e relatórios.

## 🎯 Sobre o Projeto

Este projeto realiza uma análise de crédito automatizada para empresas listadas na B3, utilizando diversos indicadores financeiros para gerar um score e rating. O sistema produz relatórios detalhados em Excel e PDF, facilitando a visualização e compartilhamento dos resultados.

## 🚀 Como Usar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/analise-credito-b3.git
cd analise-credito-b3
```

2. Instale as dependências:
```bash
pip install pandas numpy matplotlib fpdf xlsxwriter
```

3. Prepare seu arquivo CSV com os dados das empresas (veja formato abaixo)

4. Execute o notebook `AnaliseCred_cnpj.ipynb`

## 📊 Indicadores Utilizados

- Liquidez Geral
- Endividamento Relativo
- Rentabilidade Média (ROIC e ROE)
- Margem Média (EBIT e Líquida)
- Crescimento em 5 anos

## 🏆 Sistema de Rating

| Rating | Score | Descrição |
|--------|--------|-----------|
| A | >= 80 | Excelente situação financeira |
| B | >= 65 | Boa situação financeira |
| C | >= 50 | Situação financeira regular |
| D | < 50  | Situação financeira que requer atenção |

## 📁 Formato do CSV

O arquivo de entrada deve conter as seguintes colunas:
```
Papel,EV/EBITDA,MrgEbit,MrgLiq,LiqCorr,ROIC,ROE,Liq2meses,PatrimLiq,DivBrut/Patrim,Cres_Receita5a
```

## 📦 Estrutura do Projeto

```
analise-credito-b3/
├── AnaliseCred_cnpj.ipynb
├── dados_credito_b3.csv
└── output_credito_pdf/
    ├── excel/
    │   └── analise_credito.xlsx
    └── pdf/
        └── analise_credito.pdf
```

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.
