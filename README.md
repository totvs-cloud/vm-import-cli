# CLI VM IMPORT
Objetivo CLI VM Import

1. Realizar upload arquivo OVF para o Bucket;
2. O VM Import apresenta o progresso do upload;
3. Ao finaliza o upload demonstra em tela a conclusão da importação;

----------------------------------------------------------------

## Estrutura config.json
```
{
  "Bucket": "bck_name",
  "AccessKeyID": "usr_key",
  "SecretAccessKey": "scr_key"
}
```

## Execução CLI VM Import
```
vm-import -config config.json -file arquivo.ovf -check-sha256 true
```
