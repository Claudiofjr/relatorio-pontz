# Gerador de Relatório — Pontz

Página web simples: você cola o texto bruto de uma proposta, clica em **Criar relatório** e recebe o relatório formatado, pronto para copiar.

## O que a página faz

1. Lê o texto colado no campo.
2. Extrai os campos (rótulo na linha, valor na linha seguinte):
   - CPF/CNPJ do Cliente
   - Nome do Cliente
   - Data de nascimento
   - Telefone/celular
   - E-mail
   - Renda
   - Crédito
   - Endereço
3. Extrai outros dados dentro do texto:
   - **Contrato** ← `Proposta <número>`
   - **Grupo** ← `Grupo - <número>`
   - **Cota** ← `Cota - <número>`
4. Procura o CEP no endereço e consulta a [ViaCEP](https://viacep.com.br) para preencher **Cidade/UF**.
5. Monta o relatório:

```
Administradora: Pontz
Contrato:
Grupo:
Cota:
Crédito:
Forma de pagto:
Lead?:
CPF:
Nome:
Data Nasc.:
Telefone:
E-mail:
Renda:
Cidade/UF:
```

6. Exibe na tela com o botão **Copiar relatório**.
