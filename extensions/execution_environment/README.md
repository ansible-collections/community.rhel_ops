Build EE manually, push to quay.io

```
ansible-builder build
# podman build -f context/Containerfile -t ansible-execution-env:latest context
podman tag ansible-execution-env:latest quay.io/justinc1_github/apd-ee-25-experience:latest
podman push quay.io/justinc1_github/apd-ee-25-experience:latest
```