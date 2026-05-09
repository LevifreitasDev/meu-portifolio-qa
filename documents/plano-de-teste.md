Projeto: E-commerce teste

QA Responsável: Levi Freitas

Contexto: Validação de comportamento de diferentes perfis de usuário.

1. Objetivo
   Garantir que o sistema de autenticação direcione os usuários corretamente e que a interface de produtos exiba informações íntegras e confiáveis para o cliente final.

2. Escopo de Testes Manuais
   Funcionalidade: Tela de Login (entrada de dados e botões).

Funcionalidade: Vitrine de Produtos (exibição de imagens, títulos e descrições).

3. Cenários Mapeados
   CT-01: Autenticação de Usuário Padrão
   Objetivo: Verificar se um usuário comum consegue acessar a loja.

Resultado: Login efetuado com sucesso e redirecionamento para a página de produtos.

Status: Passou.

CT-02: Integridade de Dados (Perfil Problemático)
Objetivo: Verificar se a interface mantém a consistência visual com o perfil problem_user.

Resultado: Falha crítica na exibição de ativos (imagens de cachorros no lugar dos produtos) e vazamento de strings de código nas descrições.

Status: Falhou (Bug Reportado).

4. Gestão de Defeitos (Resumo do Bug)
   ID do Bug: [Produtos] Informações erradas e duplicatas de fotos.

Severidade: Grave.

Impacto: A experiência do usuário é totalmente quebrada, impedindo a visualização correta do catálogo de vendas.

5. Critérios de Aceitação
   O sistema deve exibir apenas imagens vinculadas ao ID correto do produto.

As descrições não devem conter trechos de código ou caracteres especiais de programação.

A página de produtos deve carregar em menos de 2 segundos após o login.
