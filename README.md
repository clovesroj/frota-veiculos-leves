# Frota de Veículos Leves

Painel da relação de frota de veículos leves da **CRV Industrial · Unidade Capinópolis - MG · Departamento Agrícola**,
montado a partir da planilha *Relação de frota veículos leves* (posição de 10/11/2026).

É um arquivo único, [`frota-veiculos-leves.html`](frota-veiculos-leves.html): abra com dois cliques no Edge ou no Chrome.
Não precisa instalar nada nem de servidor. A internet só é usada para as fontes e para ler/gerar Excel.

## O que tem

| Aba | Conteúdo |
|---|---|
| **Resumo** | Indicadores (na relação, em operação, saem da operação, vendidos, pendências), composição por categoria e marca, gráficos por setor, modelo e área, quadro setor × área por categoria |
| **Detalhamento** | Lista completa, agrupada por seção da planilha, setor, área, categoria ou modelo; ordenação por coluna; chassi, RENAVAM e proprietário opcionais |
| **Conferência de cadastro** | Chassi e RENAVAM repetidos, chassi sem 17 caracteres, fabricante do chassi (WMI) diferente da marca, dígito verificador do RENAVAM, placa fora do padrão, vendido ainda na relação, veículo sem usuário |
| **Alterações** | Histórico do que foi editado no painel e ainda não foi exportado |

- **Filtros** por situação, vínculo, setor, área, categoria, modelo e UF, e busca por frota, placa, usuário ou chassi. Clicar numa barra, categoria ou indicador também filtra.
- **Edição:** clique num veículo para editar ou use *Novo veículo*. Placa, chassi e RENAVAM são conferidos enquanto se digita.
- **Impressão:** botão *Imprimir* escolhe as partes (resumo, detalhamento, conferência), filtro atual ou relação inteira, paisagem ou retrato.
  O relatório tem layout próprio para A4: o resumo cabe numa folha (indicadores, composição, setores, modelos e o quadro por setor e área em colunas),
  o detalhamento sai em tabela compacta com o cabeçalho repetido em cada página, e as margens trazem cabeçalho e rodapé com posição da planilha e número da página.
  Com a relação atual, o relatório completo em paisagem tem 5 páginas (resumo 1, detalhamento 2, conferência 2). Para PDF, use *Salvar como PDF*.
- **Tema** claro e escuro.

## Atualizar os dados

1. Atualize a planilha no Excel, mantendo o formato (cabeçalho `Item | Item Setor | Frota | Placa | …`, seções 1, 2 e 3 e a aba `VENDIDOS`).
2. No painel, clique em **Importar planilha** (ou arraste o arquivo para a janela).

As edições feitas no painel ficam guardadas **só no navegador e no computador onde foram feitas**.
Para guardar de vez ou enviar a alguém, use **Exportar Excel**: o arquivo sai no mesmo formato da planilha original
(mais as abas `RESUMO` e `PENDÊNCIAS`) e pode ser importado de volta.

## Regras de classificação

- **Categoria** (pelo modelo): Picape (Strada, Saveiro, Toro, Oroch), Moto (Honda NXR, Yamaha Crosser), Passeio (Gol, Mobi, Polo),
  Utilitário (Spin, ambulância). Pode ser trocada à mão na edição do veículo.
- **Situação** (pela seção da planilha): seção 1 e 3 = em operação, seção 2 = sai da operação, aba Vendidos = vendido.
- **Vínculo:** seções 1 e 2 = Departamento Agrícola; seção 3 = Administração e Indústria.

## Dados

O arquivo traz embutidos os dados da planilha (nomes de usuários, placas, chassis e RENAVAM).
Mantenha este repositório **privado**.
