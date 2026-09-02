# Burocracia Adulta — base de regras

Arquivo `rules.json` que o app Burocracia Adulta baixa para manter prazos, calendários e checklists
atualizados sem depender de versão nova na App Store.

- `version`: data ISO (`AAAA-MM-DD`, opcionalmente com letra). O app só troca se a versão for maior, como texto.
- `rules`: por tipo de documento (prazo para começar a agir, checklist com dias antes, custo, onde, dica, se é anual).
- `states`: por UF, calendário de IPVA e licenciamento 2026 por final de placa, com fonte.
- `cities`: IPTU 2026 de capitais.
- `passportDestinations`: meses de validade exigidos por destino.
- `validity`: validade da CNH e do passaporte pela idade na emissão; garantia legal.

Toda mudança deve vir com fonte oficial no campo `source`/`note`. Um arquivo inválido é descartado pelo app.
