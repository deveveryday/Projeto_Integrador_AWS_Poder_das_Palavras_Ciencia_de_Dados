# AWS - O Poder das Palavras 💻

######  Projeto Integrador desenvolvido no Centro Universitário UniSenai, no curso de Inteligência e Análise de Dados.


###### Integrantes: Ana, Gabriel e Justino

> Este projeto visa analisar qual a relação entre a Avaliação do usuário e o comentário do mesmo.
> Para isso foram utilizadas algumas bibliotecas que mostram uma numeração conforme a detecção sobre um texto ser positivo ou negativo.
> Também foi desenvolvida uma função prória para efetuar a mesma detecção.
> Posteriormente foi efetuada uma EDA com os dados.
> Além dos comentários, os conjuntos de dados também mostram dados como Produtos, Vendedores e Localização
> Os dados tratados e já avaliados são disponibilizados em um arquivo Parquet: aws.parquet

---

## Conceito Geral

> Aplicar os conhecimentos de Python e Análise Descritiva Exploratória para devolver uma solução para Amazon

## Files

* Python Notebook: project_eda_aws_100426.ipynb
* Dicionário de Dados: 
* DER: Arquitetura_de_Dados_DER_aws_shop.drawio.svg
* Apresentação: Presentation.pdf

## Implementação

 Exemplo de PLOT para análise
```
plt.figure(figsize=(10, 6))
sns.violinplot(x="review_score", y="review_text_vader", data=df_parquet, inner="quartile", palette="viridis", hue="review_score", legend=False)
plt.title("Comportamento da biblioteca Vader em relação a nota dada pelo usuário")
plt.xlabel("Review Score (1-5)")
plt.ylabel("Vader Score (1-5)")
plt.grid(axis="y", linestyle="--")
plt.show()
```


## Ideia para AWS

Conforme a nota da avaliação resultande das bibliotecas, rodar uma função para exibir produtos, banners e outras informações para tentar fidelizar ou efetuar outra venda para este usuário

Tks, Justino! 🚀
