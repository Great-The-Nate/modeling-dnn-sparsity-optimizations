This repository builds significantly off of the work done by the Accelergy Project with Sparseloop (https://github.com/Accelergy-Project/micro22-sparseloop-artifact). 

## System requirement
### Step 0: Prepare your `docker-compose.yaml`
-------------------------

- Create a docker compose file by making a copy of the docker compose tempalte file `cp docker-compose.yaml.template docker-compose.yaml` 
- Examine the instructions in `docker-compose.yaml` to setup the docker correctly, i.e., setup the correct `UID` and `GID`.


### Step 1: Get the docker
---------------------

We provide two options for obtaining the docker image. Please choose one of the methods listed below.

- We provide a pre-built image on dockerhub
  ```
  docker-compose pull
  ```

### Step 2: Start the docker
--------------------

- Run `docker-compose up`. You should see the docker being setup.
- This docker uses Jupyter notebooks, and you will see an URL once the docker is up. Please copy and paste the `127.0.0.1 URL`
to a web browser of your choice to access the workspace. 
- If you are experiencing any issues when bringing the page up, please try the tourble shooting notes in `docker-compose.yaml`.

### Step 3: Run experiments in the docker
--------------------

We provide a jupyter notebook for the experiments.  Please navigate to `workspace/2022.micro.artifact/notebook` to run the experiments. Each cell in the notebook provides the background, instructions, and commands to run each evaluation with provided scripts.