#!/bin/bash

# Definindo parametros do sistema
DATE=`date +%d-%m-%Y`
MYSQLDUMP=/usr/bin/mysqldump
BACKUP_DIR=(DIRETORIO DO BACKUP)
BACKUP_NAME=NOMEDOBACKUP-$DATE.sql

#Gerando arquivo sql
$MYSQLDUMP -u (USUARIO DO BANCO) -p(SENHA DO BANCO) (NOME DO BANCO) > $BACKUP_DIR/$BACKUP_NAME
