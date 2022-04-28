!Acessar o modo EXEC Privilegiado (enable)
 
   !Configurar a data e hora do Switch
   clock set 19:30:00 April 2022

   !Modo de configuração global (configure terminal)

      !configuração do hostname (Nome do Equipamento)
      hostname sw-01

      !Habilitar criptografia de senha
      service password-encryption

      !Habilitar a marcação de data de hora do log
       service timestamps log datetime msec

       !desativar a resolução de Nome
       no (desativa o serviço de nome)
       no ip domain-lookup

       !configuração da mensagem do dia 
       banner motd #AVISO acesso autorizado somente a funcionarios# 

       !Habilitando a senha do modo enable 
       enable secret 123@senac 

       !criar Usuario de administração do Switch
       username senac secret 123@senac 

       !acessar a linha de console 
       line console 0

       !fazer login local 
       login local

       !Habilitando o sincronismo dos logs
       logging synchronous 

       !Habilitando o tempo de inatividade
       exec-timeout 5 30

       !sair de todos os Modos
       end (ou Ctrl+Z)
    !Salvando as configuração do Switch
    copy running-config startup-config    

    !verificando as configurações do Switch
    show running-config 
    ===============Segundo Switch==============

    !Acessar o modo EXEC Privilegiado (enable)
 
   !Configurar a data e hora do Switch
   clock set 20:09:00 April 2022

   !Modo de configuração global (configure terminal)

      !configuração do hostname (Nome do Equipamento)
      hostname sw-02

      !Habilitar criptografia de senha
      service password-encryption

      !Habilitar a marcação de data de hora do log
       service timestamps log datetime msec

       !desativar a resolução de Nome
       no (desativa o serviço de nome)
       no ip domain-lookup

       !configuração da mensagem do dia 
       banner motd #AVISO acesso autorizado somente a funcionarios# 

       !Habilitando a senha do modo enable 
       enable secret 123@senac 

       !criar Usuario de administração do Switch
       username senac secret 123@senac 

       !acessar a linha de console 
       line console 0

       !fazer login local 
       login local

       !Habilitando o sincronismo dos logs
       logging synchronous 

       !Habilitando o tempo de inatividade
       exec-timeout 5 30

       !sair de todos os Modos
       end (ou Ctrl+Z)
    !Salvando as configuração do Switch
    copy running-config startup-config    

    !verificando as configurações do Switch
    show running-config 

    








