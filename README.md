# ClimaGest 2.0 — MVP funcional local

## O que está pronto
Aplicativo responsivo em português, sem instalação de dependências, com:
- Dashboard com indicadores calculados dos registros locais.
- Cadastro e exclusão de clientes.
- Ordens de serviço com estados, valor e impressão/salvar como PDF pelo navegador.
- Calculadora simplificada de BTUs.
- Biblioteca com três textos técnicos iniciais imprimíveis.
- Treinamentos demonstrativos e registro de conclusão.
- Chamados de suporte locais.
- Oportunidades da central com aceite demonstrativo.
- Configurações, exportação/importação JSON e limpeza de dados.

## Executar
Abra `index.html` no navegador (ou hospede os três arquivos `index.html`, `styles.css` e `app.js` juntos em um servidor estático). Não é necessário npm. No celular, a maneira mais simples é publicar a pasta no Netlify Drop ou GitHub Pages. Para usar Netlify Drop, extraia o ZIP e envie a pasta do projeto.

## Limitações IMPORTANTES
Este é um **protótipo funcional local**, não um SaaS pronto para clientes reais.
- `localStorage` guarda dados somente no navegador/dispositivo; limpeza do navegador pode apagá-los. Exporte backup regularmente.
- Troca de perfis é apenas demonstração. Não há autenticação, contas, isolamento multiempresa ou autorização.
- Não há pagamentos, assinatura real, e-mails, vídeos privados, notificações, emissão de nota fiscal ou distribuição automática.
- A impressão usa a função do navegador; para gerar PDF selecione "Salvar como PDF" no diálogo de impressão.
- Não coloque dados pessoais reais de clientes ou dados confidenciais neste MVP.
- A calculadora de BTUs usa regra de bolso; exige dimensionamento profissional antes de instalar equipamentos.
- Materiais e cursos são exemplos iniciais, não certificação profissional.

## Roteiro de comercialização
1. Migrar para React/TypeScript ou manter frontend estático com API.
2. Criar autenticação real e esquema multiempresa no Supabase/Postgres com RLS e testes de isolamento.
3. Armazenar arquivos privados com políticas por assinatura; disponibilizar biblioteca e LMS.
4. Implementar gateway de pagamentos, webhooks verificados, planos e controle de acesso.
5. Criar portal de cliente e fluxo de encaminhamento de OS com autorização, geografia, comissão e auditoria.
6. Configurar domínios, backups, termos, LGPD, suporte e testes automatizados.
7. Realizar homologação antes de oferecer planos pagos.

## Estrutura
- `index.html`: entrada
- `styles.css`: identidade visual e layout
- `app.js`: lógica do protótipo e persistência local

© ClimaGest — protótipo de desenvolvimento.
