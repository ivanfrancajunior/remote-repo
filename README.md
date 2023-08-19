 # RESUMO GIT/GITHUB



## Alterando mensagem dos commits

 ```git commit --amend: ```
  
        Realiza alterações com no commit usando uma interface no vim, vale lembrar que após alterações usar :wq para sair da interface.

 ```git commit --amend -m:``` 
 
    Realiza alterações com no commit sem o uso da interface, logo depois abrir as aspas e commitar normalmente.

## Desfazendo commits

Do basicão, você reseta a alteração realizada com base na hash do commit, vc acessa a hash com ``` git log```, e depois faz as alterações em 3 modalidades **--soft, --mixed e --hard**. 

o comando fica  
``` git reset --soft | --mixed | --hard ```
    
    --soft:  Reseta as alterações realizadas posteriores a hash passada.

    --mixed: Reseta as demais alterações inclusive a passada na hash, porem as mantêm no stage area para serem alteradas caso assim seja necessário

    --hard: Reseta todas as alterações anteriores, desfazendo os commits e alterações entre no intervalo caso haja. 

## Baixando e Enviando alterações ao remoto

Estando tudo comitado, alterações todas certinhas fazer o envio

``` git push + branch desejada``` 