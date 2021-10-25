# this image is built and updated weekly
# https://github.com/cse-labs/codespaces-images

FROM ghcr.io/cse-labs/k3d:latest

# some images require specific values
ARG USERNAME=vscode
ENV PATH $PATH:/home/${USERNAME}/.dapr/bin

# Added Gitops CLI
RUN curl -L "https://github.com/weaveworks/weave-gitops/releases/download/v0.3.3/gitops-$(uname)-$(uname -m)" -o gitops && \
    chmod +x gitops && \
    mv ./gitops /usr/local/bin/gitops
