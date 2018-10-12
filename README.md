# demo-mongodb
Demonstração do uso do mongoDB
# service mongod start
serve para iniciar o mongoDb
# service mongod stop
serve para parar o mongoDB
# mongo
serve para conectar ao mongoDBgit
# codigos de manuseio dentro do mongDB
# use <database>
serve para conectar a uma determinada base de dados
# db.<collection>.find()
serve para pesquisar uma collection
# db.<collection>.find().pretty()
retorna os dados da collection de forma identada
# db.<collection>.find({json}).pretty()
retorna os dados da collection de forma identada e com os parametros no find em forma de json
# db.<collection>.insert({json})
serve para inserir os dados na collection
# db.<collection>.update({filtro},{alterações})
serve para fazer uma alteração em um determinado dado
onde no filtro passa o dados que deseja alterar e em alterações coloca-se os dados alterados 
# db.<collection>.updateOne({filtro},{$set{alteracao}})
serve para fazer uma alteração em um determinado dado
onde no filtro passa-se o dado que deseja alterar e em $set você colocar entre o json apenas o dado que deseja alterar e não todos como no update normal.
# db.<collection>.remove({_id:ObjectId("id do objeto")})
serve para remover um determinado objeto
# mongodump --out <pasta>
serve para realizar um backup do seu banco de dados em uma determinada pasta
# mongorestore -h <host> -d <database> -u <user> -p <password> <pasta>
serve para restaurar um determinado banco de dados que tena sido feito um backup anteriomente
-h <host> : Nome do host
-d <database> : nome do BD
-u <user> : nome do usuário
-p <password> : senha do BD
<pasta> : pasta onde esta o arquivo a ser resaturado  <file>.bson
# mongo <host>/<database> -u <user> -p <password>
serve para conectar a um banco de dados que estiver online do domngodb
