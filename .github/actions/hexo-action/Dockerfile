FROM node:13-alpine

LABEL version="1.0.0"
LABEL repository="https://github.com/SymbioticLab/SymbioticLab.github.io"

RUN apk add --no-cache git openssh > /dev/null

COPY setup_deploy_repo.js /setup_deploy_repo.js

COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh


ENTRYPOINT ["/entrypoint.sh"]
