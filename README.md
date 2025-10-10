Disponibilizamos um pipeline aberto para mensurar Coerência Comunicacional (CC) — alinhamento semântico título↔resumo — em artigos científicos.

O repositório reúne notebooks prontos para uso (plug-and-play) com SBERT e OLS robusto, permitindo replicar, auditar e estender a pesquisa em outras áreas do conhecimento.

Franework de Coerência Comunicacional (CC)
<p align="center">
  <img src="Framework_CC.jpg">
</p>

Pipeline de Coerência Comunicacional (CC)
<p align="center">
  <img src="Pipeline_CC.jpg">
</p>

Por que usar?
1) Métrica replicável de CC aplicável além da Contabilidade.
2) Pipeline modular: da limpeza à modelagem e visualização.
3) Ciência aberta: scripts documentados e resultados auditáveis.

Replique rapidamente! 
1) Baixe/Clone este repositório.
2) Coloque o CSV exportado da Scopus na mesma pasta dos notebooks.
3) Leias as instruções de cada script antes de rodar.
4) Os resultados (tabelas e figuras) são salvos em .csv/.xlsx/.png.
5) Entrada mínima (Scopus): Title, Abstract, Author Keywords, Cited by, SJR Quartile, Year, Country.
6) Saídas típicas: dicionário temático, classificação por eixo, score de CC, estatísticas, gráficos.

Dependências:
1) Python 3.10+
2) pandas, numpy, sentence-transformers, scikit-learn, statsmodels, matplotlib
3) Dica rápida: pip install -U pandas numpy sentence-transformers scikit-learn statsmodels matplotlib

Como contribuir / replicar:
1) Use este repositório como base de comparação (fork).
2) Adapte o CSV para outros domínios (Saúde, Educação, ESG, TI público).
3) Compartilhe issues com novos eixos temáticos, thresholds ou modelos de linguagem.

Citação:
G.O & Rosa (2025)
