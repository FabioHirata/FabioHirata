# Fabio Hirata
### Entre pessoas, operações e tecnologia.

Transformo rotinas de operação em interfaces claras, regras testáveis e ferramentas que você pode explorar. Aqui, os projetos mostram o trabalho: experimente a interface, leia as decisões e confira o código.

**[Site pessoal e contato](https://fabiohirata.github.io/fabio-hirata-site/)** · **Português / English / 日本語**

---

## Projetos em destaque

### 01 · Turno
**Planejamento de equipe com regras que acompanham cada alteração.**

Uma escala semanal que cruza disponibilidade, cobertura e carga horária. A interface mostra onde faltam pessoas e quais atribuições precisam de revisão.

- **Experimente:** ajuste os turnos, resolva conflitos e exporte a escala.
- **Por dentro:** API REST em **Go**, frontend **JavaScript**, persistência JSON com escrita atômica e revisões para evitar sobrescritas em edições concorrentes.
- **Decisão de projeto:** modo de demonstração independente; no modo API, o servidor valida as alterações e calcula os relatórios.

**[Abrir demo ↗](https://fabiohirata.github.io/turno-shift-planner/)** · [Código, arquitetura e execução local](https://github.com/FabioHirata/turno-shift-planner) · [Testes e verificação](https://github.com/FabioHirata/turno-shift-planner/blob/main/docs/QA.md)

<details>
<summary>Ver a interface · Turno</summary>

<p>Captura do modo API Go executado localmente, com dados fictícios.</p>
<img src="https://raw.githubusercontent.com/FabioHirata/turno-shift-planner/main/docs/api-go-pt.png" width="720" alt="Turno: escala semanal, indicadores de cobertura, alertas e disponibilidade da equipe fictícia">

</details>

---

### 02 · Forno
**Pedidos organizados, com a capacidade de produção à vista.**

Um balcão de encomendas para uma padaria fictícia. Catálogo, preço, produção do dia e andamento do pedido ficam no mesmo fluxo.

- **Experimente:** crie uma encomenda, teste o limite diário e acompanhe seu status.
- **Por dentro:** **JavaScript, HTML e CSS**, regras de domínio isoladas, valores em ienes inteiros e persistência versionada no navegador.
- **Decisão de projeto:** cancelar libera capacidade; reativar um pedido exige validar o limite novamente. Exportação CSV inclui proteção contra fórmulas.

**[Abrir demo ↗](https://fabiohirata.github.io/forno-order-desk/)** · [Código e decisões](https://github.com/FabioHirata/forno-order-desk) · [Testes e verificação](https://github.com/FabioHirata/forno-order-desk/blob/main/docs/QA.md)

<details>
<summary>Ver a interface · Forno</summary>

<img src="https://raw.githubusercontent.com/FabioHirata/forno-order-desk/main/docs/desktop-pt.png" width="720" alt="Forno: formulário de encomenda, capacidade diária e quadro de pedidos fictícios">

</details>

---

### 03 · Service Watch
**Observações de serviços e histórico de incidentes, sem perder o contexto.**

Uma central de operações que reúne indicadores, janelas de observação e acompanhamento de incidentes.

- **Experimente:** explore as métricas ilustrativas e registre a evolução de um incidente.
- **Por dentro:** coletor HTTP e API em **Python**, armazenamento transacional **SQLite** e frontend **JavaScript**.
- **Decisão de projeto:** no backend local, a coleta é real e manual, com destinos explicitamente permitidos e limites de tempo. Encerrar um incidente preserva as observações históricas.

**[Abrir demo ↗](https://fabiohirata.github.io/service-watch/)** · [Código, arquitetura e execução local](https://github.com/FabioHirata/service-watch) · [Testes e verificação](https://github.com/FabioHirata/service-watch/blob/main/docs/QA.md)

<details>
<summary>Ver a interface · Service Watch</summary>

<p>Captura da demonstração estática, com métricas e serviços fictícios.</p>
<img src="https://raw.githubusercontent.com/FabioHirata/service-watch/main/docs/desktop-pt.jpg" width="720" alt="Service Watch: indicadores ilustrativos, gráficos de observações e registro de incidentes fictícios">

</details>

---

### O que conecta os projetos

**Regras de negócio explícitas · Interfaces responsivas · PT / EN / 日本語 · Testes de domínio · Documentação das decisões**

As demos públicas usam cenários fictícios e funcionam no navegador. **GitHub Pages não executa os backends Go e Python**: os repositórios explicam como rodá-los localmente. São projetos de portfólio, sem clientes ou operação em produção alegados. Não insira dados pessoais.

<details>
<summary><strong>English · Explore the projects</strong></summary>

## Practical tools for everyday operations

I turn operational workflows into clear interfaces, testable rules and tools you can explore.

- **[Turno](https://github.com/FabioHirata/turno-shift-planner)** — Weekly shift planning with availability and coverage checks. Go REST API, atomic JSON persistence, optimistic revisions and a JavaScript frontend. [Try the demo](https://fabiohirata.github.io/turno-shift-planner/).
- **[Forno](https://github.com/FabioHirata/forno-order-desk)** — A fictional bakery order desk with pricing, daily capacity, order statuses and CSV export. JavaScript with isolated business rules and browser storage. [Try the demo](https://fabiohirata.github.io/forno-order-desk/).
- **[Service Watch](https://github.com/FabioHirata/service-watch)** — A Python HTTP collector/API, transactional SQLite storage and a JavaScript incident dashboard. Manual local collection preserves observations separately from incident history. [Try the demo](https://fabiohirata.github.io/service-watch/).

All three interfaces support Portuguese, English and Japanese. Public demos use fictional data; GitHub Pages does not run the Go or Python backends. Local setup, tests and limitations are documented in each repository. These are portfolio projects, not claimed client deployments or production services.

[Personal website and contact](https://fabiohirata.github.io/fabio-hirata-site/)

</details>

<details>
<summary><strong>日本語 · プロジェクトを見る</strong></summary>

## 日々の業務を、わかりやすいツールに

業務の流れを、使いやすい画面と検証可能なルールを備えたツールにしています。デモとソースコードから、実装と設計の考え方をご覧いただけます。

- **[Turno](https://github.com/FabioHirata/turno-shift-planner)**：勤務可能な時間帯と必要人数を確認できる週間シフト管理。GoのREST API、アトミックなJSON保存、同時編集の競合検出、JavaScriptの画面を備えています。[デモを開く](https://fabiohirata.github.io/turno-shift-planner/)。
- **[Forno](https://github.com/FabioHirata/forno-order-desk)**：架空のベーカリーの注文管理。料金計算、日別の生産枠、注文状況、CSV出力をまとめています。JavaScriptの業務ロジックを画面処理から分離し、データはブラウザに保存します。[デモを開く](https://fabiohirata.github.io/forno-order-desk/)。
- **[Service Watch](https://github.com/FabioHirata/service-watch)**：PythonのHTTPコレクター・API、SQLite、JavaScriptを組み合わせたサービス状況・インシデント管理。ローカル環境で手動収集し、観測データと対応履歴を分けて保存します。[デモを開く](https://fabiohirata.github.io/service-watch/)。

3つの画面はポルトガル語・英語・日本語に対応しています。公開デモは架空データを使用します。GitHub PagesではGo・Pythonのバックエンドは動作しません。ローカルでの実行方法、テスト、制約は各リポジトリに記載しています。実際の顧客向け導入事例や本番サービスを示すものではありません。

[個人サイト・お問い合わせ](https://fabiohirata.github.io/fabio-hirata-site/)

</details>
