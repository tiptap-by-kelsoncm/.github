# Como contribuir / How to contribute

[Português (Brasil)](#português-brasil) · [English](#english)

## Português (Brasil)

Obrigado pelo interesse! Este projeto é **comunitário e não oficial**: não tem afiliação com a Tiptap GmbH. Leia o [Código de Conduta](CODE_OF_CONDUCT.md) antes de participar.

### Relatar um problema ou sugerir algo
1. Procure nas issues do repositório (`tiptap-core`, `tiptap-webcomponent` ou `tiptap-ng`) se já existe algo igual.
2. Abra uma issue usando o modelo (bug ou sugestão). Informe a versão do pacote, o navegador, o framework (se houver) e os passos para reproduzir.
3. Problemas do editor do Moodle vão no [moodle-editor_tiptap](https://github.com/moodle-by-kelsoncm/moodle-editor_tiptap/issues).
4. Para **vulnerabilidades**, não abra issue pública: siga o `SECURITY.md` do repositório.

### Enviar código
1. Abra (ou comente) uma issue antes de uma mudança grande.
2. Faça um *fork* e crie uma branch a partir da `main` (sugestão: `issues/<número da issue>`).
3. Use TypeScript estrito, sem dependências novas sem justificativa. Recursos que servem a qualquer integração vão no `tiptap-core`; o web component e o componente Angular são camadas finas.
4. Escreva ou atualize **testes** (Vitest) e a **documentação** (README, `CHANGELOG.md` e, no core, o site em `site/`).
5. Rode `npm run lint`, `npm run typecheck` (quando houver) e `npm test` antes do pull request.
6. Aumente a versão em `package.json` quando o comportamento mudar.
7. Abra o pull request. O CI (lint, testes e build) precisa passar.

### Mensagens de commit
Usamos *Conventional Commits* detalhados, em português: `tipo(escopo): [TAG] Descrição no imperativo`, com `[ADD]`, `[FIX]`, `[UPD]`, `[DEL]` ou `[UPG]`, e um corpo com **Motivo**, **Impacto** e **Arquivos/Mudanças**. Contribuições em inglês também são aceitas.

### Licença
Ao contribuir, você concorda que seu código será distribuído sob a licença do repositório (**MIT**).

## English

Thanks for your interest! This is a **community, unofficial** project, with no affiliation with Tiptap GmbH. Please read the [Code of Conduct](CODE_OF_CONDUCT.md) first.

### Report a problem or suggest something
1. Search the repository's issues (`tiptap-core`, `tiptap-webcomponent` or `tiptap-ng`) for duplicates.
2. Open an issue using the template (bug or suggestion). Include the package version, browser, framework (if any) and steps to reproduce.
3. Issues of the Moodle editor go to [moodle-editor_tiptap](https://github.com/moodle-by-kelsoncm/moodle-editor_tiptap/issues).
4. For **vulnerabilities**, do not open a public issue: follow the repository's `SECURITY.md`.

### Send code
1. Open (or comment on) an issue before a large change.
2. Fork and branch from `main` (suggestion: `issues/<issue number>`).
3. Use strict TypeScript, with no new dependency without a reason. Features useful to any integration go into `tiptap-core`; the web component and the Angular component are thin layers.
4. Write or update **tests** (Vitest) and the **documentation** (README, `CHANGELOG.md` and, in the core, the site in `site/`).
5. Run `npm run lint`, `npm run typecheck` (when available) and `npm test` before the pull request.
6. Bump the version in `package.json` when behaviour changes.
7. Open the pull request. CI (lint, tests and build) must pass.

### Commit messages
We use detailed Conventional Commits, in Portuguese: `type(scope): [TAG] Imperative description`, with `[ADD]`, `[FIX]`, `[UPD]`, `[DEL]` or `[UPG]`, and a body with **Motivo** (reason), **Impacto** (impact) and **Arquivos/Mudanças** (files/changes). English contributions are welcome too.

### License
By contributing you agree that your code is distributed under the repository's license (**MIT**).
