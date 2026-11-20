# Melkor-Recipes

Catálogo privado de receitas do Melkor. Cada receita tem um arquivo JSON em `recipes/<nome>.json`. O Melkor pode propor uma receita para um aplicativo novo, testá-la em Podman rootless e abrir um PR depois do aceite local.

A CI valida o catálogo e testa as receitas alteradas. Ela compila o CLI Melkor a partir do arquivo de fontes fixado por SHA-256 na pré-release privada apontada por `MELKOR_VALIDADOR_TAG`. O hash fica em `MELKOR_VALIDADOR_SHA256`.

Versões para instalação são tags SSH assinadas depois da revisão. O arquivo de chaves públicas autorizadas é entregue fora do catálogo. A tag da CI serve à distribuição do validador.
