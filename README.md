# action-test

- create a repository
- create a Personal Access Token (PAT) in account_setting --> Developer_settings --> Personal access token --> token (classic) --> write and delete action check
- save the token
- `export <token_name>=<token>` to save it locally in your machine
- `echo $<token_name> | docker login ghcr.io -u <username> --password-stdin` to see `Login Succeeded` 

Commands:
- docker build -t ghcr.io/OWNER/IMAGE_NAME:TAG .    —> to build Dockerfile
- docker push ghcr.io/OWNER/IMAGE_NAME:TAG       —> to push to GitHub account packages (OWNER - account name)
- docker pull ghcr.io/OWNER/IMAGE_NAME:TAG
- docker run ghcr.io/OWNER/IMAGE_NAME:TAG 