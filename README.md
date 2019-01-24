Criagenda
================

<img src="https://www.criartsoft.com.br/assets/img/git-banner-criagenda.png">

### Organize seu negócio! Explorar recursos humanos que podem ser usados em outras tarefas com mais eficiência.

**Criagenda** é um aplicativo da web altamente personalizável que permite que seus clientes reservem
compromissos com você pela web. Além disso, fornece a capacidade de sincronizar seus dados com
Google Agenda, para que você possa usá-los com outros serviços. É um projeto de código aberto e você
pode baixar e instalar **mesmo para uso comercial**. Criagenda irá funcionar sem problemas com
seu site existente, porque ele pode ser instalado em uma única pasta do servidor e, claro,
Ambos os sites podem compartilhar o mesmo banco de dados.

### Características

O projeto foi projetado para ser flexível e confiável, de modo a atender às necessidades de qualquer
tipo de empresa. Você pode ler os principais recursos do sistema abaixo:

* Cadastro de Clientes e gerenciamento de compromissos.
* Serviços e Organização de provedores de serviços.
* Regras de fluxo de trabalho e de reserva.
* Sincronização do Google Agenda.
* Sistema de notificações por email.
* Instalação autônoma (como WordPress, Drupal, Joomla e outros sistemas web).
* Interface de usuário traduzida.
* Suporte da comunidade de usuários.

### Instalação

Como o Criagenda é um aplicativo da Web, ele é executado em um servidor da Web e, portanto, você precisará
execute os seguintes passos para instalar o sistema no seu servidor:

* Certifique-se de que seu servidor tenha Apache / Nginx, PHP e MySQL instalados.
* Crie um novo banco de dados (ou use um existente).
* Copie a pasta de origem "criagenda" no seu servidor.
* Certifique-se de que o diretório "storage" seja gravável.
* Renomeie o arquivo "config-sample.php" para "config.php" e defina suas propriedades de servidor.
* Abra seu navegador no URL nomedoseudominico\criagenda e siga o guia de instalação.
* É isso aí! Agora você pode usar o Criagenda à sua vontade.

Você encontrará o último lançamento em (https://www.criagenda.com.br).
Se você tiver problemas ao instalar ou configurar o aplicativo, dê uma olhada no
[wiki pages](https://github.com/alextselegidis/easyappointments/wiki) ou visite o
[official support group](https://groups.google.com/forum/#!forum/easy-appointments).
Você também pode relatar problemas na [página de problemas](https://github.com/criartsoft-brasil/criagenda)
e ajudar o progresso do desenvolvimento.

### Docker
Para iniciar o Criagenda usando o Docker na configuração de desenvolvimento, com os arquivos de origem montados no contêiner, execute:
```
docker-compose up
```

A implementação de produção pode ser feita alterando os valores necessários no arquivo .env (DB_PASSWORD, APP_URL, APP_PORT) e executando:
```
docker-compose -f docker-compose.prod.yml up -d
```

Os dados do banco de dados serão armazenados no volume nomeado `criagenda-data` e no armazenamento de aplicativos (logs, cache, uploads) em` criagenda-storage`.
```
docker volume inspect criagenda-storage
```

Os contêineres de produção serão reiniciados automaticamente em caso de reinicialização de falha / servidor. Para mais informações, dê uma olhada no arquivo `docker-compose.prod.yml`.

### Feedback do usuário

Quer se trate de novas idéias ou defeitos, o seu feedback é muito apreciado e será levado em consideração
consideração para as seguintes versões do projeto. Compartilhe sua experiência e discuta sua
pensamentos com outros usuários através de comunidades. Crie problemas com sugestões sobre novos recursos ou
relatório de erros.

### Traduzir o Criagenda
A partir da versão 1.0, o Criagenda suporta a interface do usuário traduzida. Se você quiser contribuir para o
processo de tradução leia o [envolver-se](https://github.com/alextselegidis/easyappointments/wiki/Get-Involved!)
página para informações adicionais.

### Lembrando-se
Este projeto é um forked https://github.com/alextselegidis/easyappointments.




