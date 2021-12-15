ssh-keygen -t rsa -f '/c/Users/wellingtongaboardi/.ssh/github' -C "wgaboardi@gmail.com"
eval "$(ssh-agent -s)"
ssh-add '/c/Users/wellingtongaboardi/.ssh/github'

#Iniciando o git
git init
git config --global user.name "Wellington L Gaboardi"
git config --global user.email "wgaboardi@gmail.com"
git remote add origin git@github.com:wgaboardi/temp_rep.git
git add .
git commit -m "Initial"
git push origin master -u