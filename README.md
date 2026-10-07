# Integridade dos Materiais Didáticos

Repositório oficial para registro de **integridade, versionamento e rastreabilidade** dos materiais didáticos utilizados no **Curso de Formação para Cuidadores de Animais**.

## Objetivo

Este repositório permite que alunos, professores e coordenação verifiquem se um arquivo recebido corresponde exatamente à versão oficial publicada.

A verificação é feita por meio de **hashes criptográficos SHA-256**.

> O SHA-256 não impede que um arquivo seja alterado. Ele permite detectar se o arquivo recebido é diferente da versão oficial registrada.

Qualquer alteração no conteúdo, páginas, imagens, metadados, compressão, proteção, marca-d'água ou assinatura digital produzirá um novo hash.

## Materiais oficiais

| Material | Versão | Data | Status |
|---|---:|---|---|
| Aula 01 — Origem e Domesticação de Cães | 1.0 | A definir | Em preparação |

Os demais materiais serão adicionados à medida que forem finalizados e publicados.

## Onde consultar

- **Hashes oficiais:** `manifests/SHA256SUMS.txt`
- **Histórico de versões:** `VERSIONS.md`
- **Como verificar um arquivo:** `docs/COMO_VERIFICAR.md`

## Fluxo de publicação

1. Finalizar e aprovar o material.
2. Identificar nome, versão e data.
3. Aplicar eventuais proteções, marca-d'água ou assinatura.
4. Gerar o PDF definitivo.
5. Calcular o SHA-256 do arquivo definitivo.
6. Registrar o hash neste repositório.
7. Distribuir o mesmo arquivo aos alunos.
8. Preservar o histórico caso uma nova versão seja publicada.

## Interpretação da verificação

**Hash igual:** o arquivo é bit a bit idêntico à versão registrada.

**Hash diferente:** o arquivo não é idêntico à versão registrada. Isso pode decorrer de uma alteração legítima, nova exportação, correção, compressão, mudança de metadados ou modificação não autorizada. Consulte o histórico de versões antes de concluir a causa.

## Observação sobre autenticidade

Um hash só é útil como referência oficial quando obtido por uma fonte confiável. Por isso, este repositório deve ser divulgado pela coordenação como o endereço oficial de verificação.

---

Este repositório registra a integridade dos materiais, mas não substitui políticas institucionais de autoria, licenciamento, distribuição ou direitos de uso.
