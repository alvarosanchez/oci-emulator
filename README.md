# oci-emulator

![Python 3.8.8](https://img.shields.io/badge/python-3.8.8-blue)
![license](https://img.shields.io/github/license/cameritelabs/oci-emulator)
![Python application](https://github.com/cameritelabs/oci-emulator/workflows/Python%20application/badge.svg)
[![codecov](https://codecov.io/gh/cameritelabs/oci-emulator/branch/main/graph/badge.svg?token=5C8SX1Q6P9)](https://codecov.io/gh/cameritelabs/oci-emulator)

oci-emulator is a mock of Oracle Cloud Infrastructure API using Flask. You can use it to test your application that integrates with OCI.

oci-emulator is available on dockerhub. To run it, just execute:

```bash
docker run -d -p 12000:12000 cameritelabs/oci-emulator:latest
```

## How to build?

### Using pyenv with pyenv-virtualenv

You also should use virtualenv to build/develop the project and I recommend the use of [pyenv](https://github.com/pyenv/pyenv) with [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) to manage multiple python environments.

```bash
pyenv update
pyenv install 3.8.8
pyenv virtualenv 3.8.8 oci-emulator
```

### Installing dependencies (Python 3.8.8)

Open your bash and run the follow command to install all the project dependencies, you just need to run the command one time

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

#### Docker 🐋

Building the docker file:

```bash
docker build . -t cameritelabs/oci-emulator:latest
```
