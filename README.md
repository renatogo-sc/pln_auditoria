Framework de Coerência Comunicacional (CC) — Auditoria & PLN

Objetivo. Disponibilizar um pipeline aberto para mensurar Coerência Comunicacional (CC) — alinhamento semântico título↔resumo — em artigos científicos.
O repositório reúne notebooks prontos para uso (plug-and-play) com SBERT e OLS robusto, permitindo replicar, auditar e estender os resultados do artigo.

<p align="center"> <img src="C:\Users\renat\OneDrive\Mestrado em Contabilidade\2025\2025.2k Revista Peru (Auditoria)/framework_cc.png" alt="Framework de Coerência Comunicacional" width="720"> </p>
Por que usar?

Métrica replicável de clareza textual (CC) aplicável além da Contabilidade.

Pipeline modular: da limpeza à modelagem e visualização.

Ciência aberta: scripts documentados e resultados auditáveis.

Replique em 10 minutos

Baixe/Clone este repositório.

Coloque o CSV exportado da Scopus na mesma pasta dos notebooks.

Abra Script_artigo.ipynb no Jupyter/Colab, edite o nome do arquivo de entrada (célula de configuração) e Execute All.

(Opcional) Rode Script_tempo.ipynb para monitorar o tempo de execução.

Os resultados (tabelas e figuras) são salvos em .csv/.xlsx/.png.

Entrada mínima (Scopus): Title, Abstract, Author Keywords, Cited by, SJR Quartile, Year, Country.
Saídas típicas: dicionário temático, classificação por eixo, score de CC, estatísticas, gráficos.

Estrutura atual do repositório

Script_artigo.ipynb — núcleo do pipeline: limpeza, dicionário, classificação, CC (SBERT) e OLS.

Script_tempo.ipynb — benchmark de execução (tempo e ambiente).

Se você organizar pastas adicionais, a estrutura recomendada é:

pln_auditoria/
  ├─ notebooks/        # .ipynb (produção)
  ├─ data/             # insumos (.csv) - fora do versionamento grande
  ├─ results/          # tabelas e figuras geradas
  └─ docs/img/         # figures do README (framework_cc.png, pipeline_cc.png)

Pipeline metodológico (visão rápida)
<p align="center"> <img src=""C:\Users\renat\OneDrive\Mestrado em Contabilidade\2025\2025.2k Revista Peru (Auditoria)\Pipeline_CC.jpg"" alt="Pipeline metodológico da CC" width="820"> </p>

Etapas: (i) palavras-chave → (ii) dicionário temático → (iii) classificação de artigos → (iv) CC título↔resumo → (v) modelagem (H1–H3).

Dependências

Python 3.10+

pandas, numpy, sentence-transformers, scikit-learn, statsmodels, matplotlib

Dica rápida: pip install -U pandas numpy sentence-transformers scikit-learn statsmodels matplotlib

Como contribuir / replicar

Use este repositório como base de comparação (fork).

Adapte o CSV para outros domínios (Saúde, Educação, ESG, TI público).

Compartilhe issues com novos eixos temáticos, thresholds ou modelos de linguagem.

Citação

Oliveira, R. G. (2025). Framework de Coerência Comunicacional (CC) — Auditoria & PLN. GitHub. https://github.com/renatogo-sc/pln_auditoria

Como colocar as figuras no README

No GitHub, clique em Adicionar arquivo → Enviar arquivos.

Envie as imagens para docs/img/ com estes nomes:

framework_cc.png

pipeline_cc.png

O README já está preparado com os caminhos relativos. Atualize a página.
