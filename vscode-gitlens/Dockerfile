FROM node:lts-alpine3.19
RUN git clone https://github.com/gitkraken/vscode-gitlens.git vscode-gitlens 
RUN npm install yarn -g
RUN yarn config set registry https://registry.npmmirror.com
RUN cd vscode-gitlens && npm install sharp --force
RUN yarn run rebuild


 