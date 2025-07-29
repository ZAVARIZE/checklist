# Sistema de Autorização - Checklist Veicular

Este repositório controla o acesso ao aplicativo **Checklist Veicular**.

## Como funciona

- O arquivo `authorized-devices.txt` contém a lista de dispositivos autorizados
- Cada linha do arquivo representa um ID único de dispositivo
- Linhas começadas com `#` são comentários e são ignoradas

## Como autorizar um novo dispositivo

1. O usuário acessa o aplicativo e vê a tela "Acesso Restrito"
2. O ID único do dispositivo é mostrado na tela
3. Adicione este ID ao arquivo `authorized-devices.txt`
4. O usuário pode recarregar a página e terá acesso

## Formato do arquivo authorized-devices.txt

```
# Comentários começam com #
# Um ID por linha

ABC123DEF456
XYZ789UVW012
```

## Solicitações automáticas

Quando um usuário não autorizado solicita acesso pelo aplicativo, uma issue é criada automaticamente neste repositório com as informações do dispositivo.
