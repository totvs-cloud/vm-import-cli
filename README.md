# Objetivo CLI VM Import
### Tipos de arquivo válidos. ###
- OVF


**Facilitar o processo de importação de virtual machine para nuvem da TOTVS.**

1. Realizar upload arquivo para o Bucket;
2. O VM Import apresenta o progresso do upload;
3. Ao finaliza o upload demonstra em tela a conclusão da importação;

----------------------------------------------------------------

# Estrutura config.json
```
{
  "Bucket": "bck_name",
  "AccessKeyID": "usr_key",
  "SecretAccessKey": "scr_key"
}

```
----------------------------------------------------------------

# Execução CLI VM Import

**Observação:** Ao baixar o CLI VM Import cerfique que é um executável.

### Exemplo Linux OS

```
./vm-import -config config.json -file arquivo.ovf -check-sha256 true
```

![image](https://user-images.githubusercontent.com/121171463/219680829-a9ec1a24-6506-4a6d-a564-d828e067179d.png)


----------------------------------------------------------------

# Erros

Mensagem                                                                                                                        | Descrição
--------------------------------------------------------------------------------------------------------------------------------|-----------------------
Resposta invalida. Digite **Y** para sim e **N** para não!                                                                      | Escolha de opção inexistente 
Arquivo de configuração informado **__NOME_ARQUIVO__**  não existe!                                                             | Nome do arquivo e ou arquivo de configuração não existe 
**__Bucket__** não encontrado. Favor informe o bucket por variaveis de ambiente ou informe o arquivo de configuração.           | Nome Bucket incorreto e ou inexistente
**__AccessKey__** não encontrada. Favor informe a AccessKey por variaveis de ambiente ou informe o arquivo de configuração.     | AccessKey incorreta
**__SecretAccessKey__** não encontrada. Favor informe a SecretAccessKey por variaveis de ambiente ou informe o arquivo de configuração.| SecretAccessKey incorreta


