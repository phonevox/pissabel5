# pissabel5
> Issabel 5 netinstall custom Ghonevox Group

Disponibilizado o arquivo em núvem para o time fazer a instalação via snippets.

## Instalação

Já com o [Rocky linux 8](https://download.rockylinux.org/pub/rocky/8/isos/x86_64/Rocky-8.10-x86_64-minimal.iso) instalado na máquina e com o tmux instalado, execute o seguinte comando: 

```bash
sudo su yum update -y && yum install tmux -y && yum install git -y && tmux new -s issabel -d "git clone https://github.com/phonevox/pissabel5.git && cd pissabel5 && chmod +x issabel5-netinstall.sh && ./issabel5-netinstall.sh"
```

## Sugestão de melhorias
- Instalação sem interação;
- Instalar sngrep;
- Ajustar "cor das pastas" (~/.bashrc) 
- Fixar versão para o Asterisk 18;
- Fixar linguagem para pt_BR;
- Alterar horário do servidor;
- Alterar timezone do PHP;
- Alterar portas padrões (sip e pjsip);
- Segurança básica, desativar login root, alterar porta ssh, liberar apenas as portas necessárias para o externo;