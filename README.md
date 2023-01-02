# dependency-track eval

https://dependencytrack.org

## Quickstart

### podman/podman-desktop, podman-compose

    ```bash
    brew install podman # and/or podman-desktop
    podman machine init --cpus 2 --memory 8096 # 2cpus/8gb is minimum
    python -m venv .venv
    . .venv/bin/activate
    pip install -r requirements.txt
    podman-compose up -d
    ```

** It will take 10-30 minutes to initially sync the various databases, do not stop the process. **

Login to the web interface at http://localhost:8080

    - username: admin
    - password: admin

You will be prompted to change the password.
