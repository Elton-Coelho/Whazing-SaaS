# Agora acesse o SSH 

- Execute o comando para atualizar o Whazing

quando chegar no comando 

**npm run build**

aperte enter para continuar

```bash
su deploy
cd /home/deploy/whazing
unzip -o whazing.zip
chmod 775 /home/deploy/whazing/ -Rf
cd backend
npm install --force
npx sequelize db:migrate
pm2 restart all
cd ..
cd frontend
npm install --force
npm run build
```

feche a página do sistema e logue novamente


Pronto seu sistema está atualizado


para verificar se atualizou 


acesse o módulo Empresas


![image](https://github.com/user-attachments/assets/b57f6419-6a67-415e-af50-577190e0c6ee)

