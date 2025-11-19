---
name: TESTE
about: TESTE SOBRE
title: "[DESAFIO]"
labels: Comunity Collection
assignees: ''

---

name: "Custom Issue"
description: "Template para relatar problemas, solicitar melhorias ou descrever novas funcionalidades."
title: "[TÍTULO BREVE] "
labels: []
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        ## 📝 Descrição
        Explique de forma clara e objetiva o que está acontecendo ou o que deseja propor.

  - type: textarea
    id: descricao
    attributes:
      label: "Descrição Detalhada"
      description: "Forneça todos os detalhes relevantes: comportamento atual, comportamento esperado, impacto, prints, logs, etc."
      placeholder: "Descreva o problema ou sugestão aqui..."
    validations:
      required: true

  - type: input
    id: passos
    attributes:
      label: "Passos para reproduzir (se aplicável)"
      placeholder: "1. Vá até...\n2. Clique em...\n3. Resultado..."
    validations:
      required: false

  - type: input
    id: esperado
    attributes:
      label: "Comportamento Esperado"
      placeholder: "Descreva o que deveria acontecer..."
    validations:
      required: false

  - type: dropdown
    id: tipo
    attributes:
      label: "Tipo de Issue"
      options:
        - Bug
        - Melhoria
        - Nova Funcionalidade
        - Documentação
        - Outro
    validations:
      required: true

  - type: textarea
    id: anexos
    attributes:
      label: "Evidências / Anexos"
      description: "Inclua prints, links, vídeos ou arquivos relevantes."
      placeholder: "Arraste e solte arquivos aqui..."
    validations:
      required: false

  - type: markdown
    attributes:
      value: |
        ---
        Obrigado por contribuir! 🚀
