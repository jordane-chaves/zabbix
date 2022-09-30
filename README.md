<h1 align="center">Instalação do Zabbix no Ubuntu</h1>

<p align="center">Automatiza a instalação do Zabbix no sistema Ubuntu.</p>

O script instala o Zabbix de acordo com a versão do Ubuntu, para o Ubuntu 18.04 será instalado a versão 5.4 do Zabbix e para versões posteriores do sistema operacional, será apresentado um menu para escolha entre as versões 5.4 ou 6.0 do Zabbix.

> Foram feitos testes apenas nas versões 18.04 e 20.04 do Ubuntu.

## Como Usar?

Acesse com o usuário root

```bash
sudo su
```

Execute o comando abaixo para efetuar a instalação:

```bash
wget https://raw.githubusercontent.com/jordane-chaves/zabbix/main/install.sh && chmod u+x install.sh && ./install.sh && rm -rf install.sh
```

> Ao iniciar o script irá solicitar que selecione a versão e a senha para ser configurada no banco de dados do zabbix.

Agora é só aguardar a instalação finalizar e ser feliz 🎉

## Logs

Verifique os logs caso ocorra algum erro:

```bash
$ tail -f /var/log/zabbix/zabbix_server.log
```

## Credenciais Padrões

**URL:** http://IP-DO-SERVIDOR/zabbix <br>
**Usuário:** Admin <br>
**Senha:** zabbix

## Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/jordane-chaves" width="100px;" alt=""/>
<br />

Feito com 💜 por Jordane Chaves
