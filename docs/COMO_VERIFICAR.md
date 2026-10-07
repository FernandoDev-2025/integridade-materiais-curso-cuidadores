# Como verificar a integridade dos materiais

Cada material oficial possui um hash SHA-256 registrado em `manifests/SHA256SUMS.txt`.

Se o arquivo recebido produzir o mesmo SHA-256 registrado neste repositório, ele é bit a bit idêntico à versão oficial registrada.

## Windows — PowerShell

Abra o PowerShell na pasta onde estão os PDFs e execute, por exemplo:

```powershell
(Get-FileHash -LiteralPath '.\AULA_ 1.pdf' -Algorithm SHA256).Hash
```

Para verificar outro arquivo, substitua o nome entre aspas.

## Linux

Execute, por exemplo:

```bash
sha256sum "AULA_ 1.pdf"
```

Para verificar todos os arquivos presentes no manifesto, salve `SHA256SUMS.txt` na mesma pasta dos PDFs e execute:

```bash
sha256sum -c SHA256SUMS.txt
```

## Como interpretar

- **Hash igual:** o arquivo é idêntico à versão oficial registrada.
- **Hash diferente:** o arquivo não é idêntico à versão registrada.

Um hash diferente não demonstra, sozinho, fraude. Pode indicar correção, nova exportação, alteração de metadados, compressão, proteção, assinatura digital ou modificação não autorizada.

Consulte também o `VERSIONS.md` para confirmar a versão e o histórico do material.

## Importante

O SHA-256 verifica integridade, não impede edição. Caso um material seja alterado oficialmente, a nova versão deve receber um novo hash e o histórico anterior deve ser preservado.
