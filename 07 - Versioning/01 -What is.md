Controle de versão em banco de dados 
==================================

Um ambiente robusto DevOps requer integração contínua para os componentes do sistema. Mas frequentemente, o database é omitido, conduzindo a problemas de versões de produção frágeis e práticas de desenvolvimento que tornam a vida dos novos programadores mais difíceis.

Nesse cenário, o profissional DBRE deve ter, entre suas atribuições, a preocupação com a gestão de componentes que formam a base dos serviços de dados da organização:

* Database schema, incluindo índices, precisam estar no controle de versão.

* Os dados que controlam a lógica de negócios, como tabelas de pesquisa, também precisam estar no controle de versão.

* Os desenvolvedores precisam criar de uma maneira fácil os databases locais.

* Bancos de dados compartilhados devem ser atualizados exclusivamente por processos controlados e dedicados a esta tarefa.



Por que controle de versão de banco de dados?
-------------------------------------------------------------------------------------------------

O controle de versão de banco de dados é o processo de controlar e documentar as alterações feitas no esquema e nos dados do banco de dados ao longo do tempo. Ele permite que você acompanhe o histórico, o estado e as dependências do banco de dados, bem como reverter ou migrar para versões diferentes, conforme necessário. O controle de versão do banco de dados também pode ajudá-lo a evitar conflitos, erros e perda de dados que podem surgir da aplicação de alterações incompatíveis ou inconsistentes ao banco de dados.


Como fazer a versão do seu banco de dados?
-------------------------------------------------------------------------------------------

Ao controlar o controle de versão do banco de dados, há várias abordagens e ferramentas que você pode usar dependendo de suas preferências, necessidades e tecnologias. Os métodos baseados em script envolvem a gravação e a execução de scripts SQL que definem e modificam o esquema e os dados do banco de dados. Esses scripts podem ser armazenados e gerenciados com um sistema de controle de versão (VCS) como Git ou SVN, com uma ferramenta como Flyway ou Liquibase aplicando-os ao banco de dados de forma sequencial e automatizada. Os métodos baseados em modelo usam ferramentas gráficas ou textuais para projetar e gerar o esquema e os dados do banco de dados. Novamente, um VCS pode armazenar e gerenciar os modelos, enquanto uma ferramenta como o SQL Server Data Tools (SSDT) ou Redgate SQL Change Automation compara e sincroniza com o banco de dados de forma declarativa e automatizada. Uma abordagem híbrida combina métodos baseados em script e modelo, dependendo da complexidade e frequência das alterações, com uma ferramenta como DBmaestro ou Datical fornecendo uma maneira unificada e automatizada de versão e implementação do banco de dados.


Como lidar com alterações de esquema?
---------------------------------------------------------------------------------

As alterações de esquema, que envolvem modificações na estrutura e definição de suas tabelas de banco de dados, colunas, índices, restrições etc., podem afetar drasticamente o desempenho, a funcionalidade e a compatibilidade do banco de dados e do código. Para garantir que essas alterações sejam implementadas com cuidado e eficiência, você deve planejá-las, testá-las e executá-las com cautela. Algumas das práticas recomendadas e dicas para lidar com alterações de esquema incluem o uso de convenções de nomenclatura descritivas e consistentes para seus objetos e scripts de banco de dados; documentar e comunicar claramente suas alterações de esquema com sua equipe e partes interessadas; Usando um sistema de controle de versão (VCS) para armazenar e revisar suas alterações de esquema; empregar uma ferramenta como DBDiff ou SchemaCrawler para comparar e verificar seu esquema em diferentes ambientes e versões; utilizar uma ferramenta como Flyway ou Liquibase para aplicar suas mudanças de esquema de forma controlada e repetível; e usando uma ferramenta como DBUnit ou Testcontainers para criar e preencher bancos de dados de teste com dados realistas, para que você possa executar testes automatizados em suas alterações de esquema antes de implantá-las na produção.


Como lidar com alterações de dados?
-----------------------------------------------------------------------------

As alterações de dados são modificações no conteúdo e nos valores de suas tabelas de banco de dados, colunas, registros, etc. e podem afetar a qualidade, a integridade e a usabilidade de seus dados. Portanto, é importante validá-los, fazer backup e restaurá-los com segurança e precisão. Para fazer isso, você deve usar regras e restrições de validação de dados para garantir consistência e precisão. Além disso, a criptografia e o mascaramento de dados devem ser usados para proteger dados confidenciais ou pessoais contra acesso ou divulgação não autorizados. As ferramentas de backup e restauração de dados devem ser usadas para criar e armazenar cópias de seus dados em caso de perda ou corrupção. Finalmente, as ferramentas de migração e transformação de dados podem ser usadas para mover e modificar seus dados em diferentes bancos de dados, formatos ou plataformas, bem como lidar com quaisquer problemas de compatibilidade ou desempenho que possam surgir.


Como monitorar e otimizar seu banco de dados?
-------------------------------------------------------------------------------------------------

Monitorar e otimizar seu banco de dados são tarefas essenciais para garantir que ele esteja funcionando bem, atendendo aos seus requisitos e se adaptando às suas mudanças. Para fazer isso, você precisa coletar e analisar dados sobre a integridade, o desempenho e o uso do banco de dados, bem como aplicar quaisquer melhorias ou ajustes conforme necessário. Você pode usar uma variedade de ferramentas e técnicas para monitorar e otimizar seu banco de dados, como ferramentas de monitoramento de desempenho de banco de dados como New Relic ou Datadog para medir e visualizar métricas; ferramentas de ajuste de banco de dados como SolarWinds ou SentryOne para identificar e otimizar gargalos; ferramentas de auditoria de banco de dados como IBM Guardium ou Imperva para rastrear e auditar atividades; e ferramentas de refatoração de banco de dados como Redgate SQL Refactor ou ApexSQL Refactor para melhorar o design.

