# Vercel Front-End

Mini app do cardápio digital para rodar separado do PDV desktop.

## O que ele faz

- Lê a rota da mesa no formato `/mesa/3/CODE123`.
- Valida a mesa no Supabase.
- Captura nome e celular do cliente.
- Lista categorias e produtos.
- Permite montar carrinho e enviar pedido.

## Estrutura

- `index.html`: entrada da aplicação.
- `src/main.js`: lógica do fluxo do cliente.
- `src/styles.css`: visual do cardápio.
- `vite.config.js`: build para Vercel.
- `vercel.json`: fallback de SPA.

## Variáveis de ambiente

Configure na Vercel:

```env
VITE_SUPABASE_URL=...
VITE_SUPABASE_PUBLISHABLE_KEY=...
```

Você também pode usar [vercel/.env.example](/C:/Users/thiag/Desktop/Programação/Sistema%20PDV/SISTEMAPDV%202.3/vercel/.env.example) como modelo local.

## Rotas esperadas

```text
/mesa/3/CODE123
```

## Deploy

1. Crie um projeto novo na Vercel apontando para a pasta `vercel/`.
2. Adicione as variáveis `VITE_SUPABASE_URL` e `VITE_SUPABASE_PUBLISHABLE_KEY`.
3. Faça deploy com o preset de Vite ou com o `buildCommand` já definido no `vercel.json`.
