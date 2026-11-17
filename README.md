# Central de Chamados SaveInCloud — Demo em PHP

Projeto **independente e não oficial**, feito como exemplo de painel de suporte técnico. Não use nomes, logotipos ou dados reais da empresa sem autorização.

## Recursos
- Dashboard com total de chamados e contadores por status
- Cadastro de chamados (cliente, assunto, prioridade, descrição)
- Busca e filtro por status
- Alteração de status (Aberto, Em andamento, Resolvido)
- Exclusão de chamados com confirmação
- Persistência em arquivo JSON, sem MySQL
- Token CSRF, escape HTML e travamento de arquivo para operações simultâneas

## Como rodar

Requer **PHP 8.1+** com extensão `mbstring` habilitada.

No terminal, dentro da pasta `saveincloud_demo`, execute:

```bash
php -S localhost:8000 -t public
```

Acesse **http://localhost:8000**.

No Windows com XAMPP, o ideal é configurar o DocumentRoot ou VirtualHost apontando para a pasta `public` (não para a raiz do projeto). A pasta `storage` deve permanecer **fora do diretório público**.

## Atenção antes de usar em produção

Esta é uma aplicação de **demonstração local**. Não há autenticação, perfis de acesso, banco de dados relacional, controle de permissões ou logs de auditoria. Não publique na internet nem use para dados sensíveis de clientes sem acrescentar essas proteções.
