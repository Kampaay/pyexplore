## Requirements

- conda (miniconda): https://docs.anaconda.com/miniconda/
 

 ## Cheat Sheet

 - vscode Select Interpreter: https://code.visualstudio.com/docs/python/environments#_working-with-python-interpreters

 ```bash

conda activate ENV_NAME

conda deactivate

conda remove --name ENV_NAME --all  # if it doesn't work, remove the directory manually (https://stackoverflow.com/questions/58736579/conda-unable-to-completely-delete-environment/58736677#58736677)

conda env list

# install or update the environment dependencies
# https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/creating-projects.html
# The --prune option causes conda to remove any dependencies that are no longer required from the environment.
conda env update --file environment.yml --prune -p ./env

# (un)install a dependency:
# update environment.yml adding/removing the dependency and run the update through the command above

# export the environment
conda env export > environment.yml

conda config --set env_prompt '({name})' # shorten conda prompt prefix: https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#specifying-a-location-for-an-environment

 ```

 ## known issues
