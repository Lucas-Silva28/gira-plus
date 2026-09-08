# Gira+

**Gira+** é uma plataforma de roletas e sorteios interativos para dinâmicas, aulas, treinamentos, apresentações, escolha de equipes e eventos.

## Principais recursos

- Roletas personalizadas e múltiplas roletas salvas
- Sorteio igualitário ou ponderado por peso
- Novos participantes com peso padrão 1
- Modelos prontos, incluindo **Par / Ímpar**, Sim / Não, Maior / Menor e Verdadeiro / Falso
- Temas visuais da roleta
- Galeria de efeitos visuais com 42 opções
- Pré-visualização e seleção de efeitos
- Áudio de giro, resultado e músicas personalizadas
- Controle de mute e volume
- Modo Apresentação com roleta grande e fechamento por X/ESC
- Tutorial guiado com navegação por botões e gesto de deslize
- Histórico e estatísticas
- Backup, restauração, lixeira e desfazer
- Compartilhamento/exportação de uma roleta
- Armazenamento local e funcionamento sem depender de backend
- Manifesto preparado para instalação como PWA

## Estrutura

```text
gira-plus/
├── index.html
├── manifest.json
├── PROJECT_CONTEXT.md
├── PROMPT_MESTRE_GIRA_PLUS.md
├── README.md
├── LICENSE
├── .gitignore
└── assets/
    ├── gira-plus-icon-180.png
    ├── gira-plus-icon-192.png
    ├── gira-plus-icon-512.png
    └── gira-plus-branding.png
```

## Executar localmente

Como o sistema é uma aplicação web, o ideal é servi-lo por um servidor HTTP local ou por uma hospedagem como Vercel. Abrir diretamente como `file://` pode limitar alguns recursos do navegador.

Exemplo com Python:

```bash
python -m http.server 8080
```

Depois acesse `http://localhost:8080`.

## GitHub

Repositório oficial:

`https://github.com/Lucas-Silva28/gira-plus`

Sugestão de fluxo:

```text
alteração → teste → commit → push → Vercel → deploy
```

## Versionamento

A versão desta entrega segue a linha **2.4.x**. Alterações futuras devem preservar a compatibilidade com os dados existentes e evitar regressões.

## PWA

O `manifest.json` e os ícones do aplicativo já estão preparados para a experiência instalável. A camada de Service Worker pode ser adicionada em uma etapa específica, depois da validação da versão estável, para não introduzir problemas de cache prematuramente.

## Licença

Este projeto está distribuído sob uma licença proprietária. Consulte `LICENSE` antes de reutilizar código ou assets.
