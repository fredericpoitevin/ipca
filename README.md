# iPCA

## Quick install

For now, it is as easy as forking and cloning:
```bash
git clone https://github.com/<your_github_handle>/ipca
```

## Usage

To be done...
`/sdf/scratch/fpoitevi/singularity_images/ana-skopi_latest.sif`

## Data Availability

To be done...

## Contributing

Tasks that need to be adressed will appear in the [Issues](https://github.com/fredericpoitevin/ipca/issues) page. Before you start contributing to solve a task, make sure you have forked this repo and develop within your own fork. Once you are done working on the issue, make a pull request.

Please pay attention to the following guidelines:

1. *Write Python scripts*: Jupyter notebooks are great for two things: 1) exploration in the initial stages of writing new code, 2) explanation in the final stages of the project. But the actual code should be stored properly in python scripts; as soon as some code is mature enough, make sure it is saved in the `src/` directory and called by the notebook from the corresponding file.

2. *Keep your master branch up to date*: when working on your own fork, it is easy to get out of sync with the main repository; remember to update your fork often in order to avoid conflicts when merging your changes. For this, you need to add the main fork as one of your "remote", like so:
```bash
git remote add fred https://github.com/fredericpoitevin/ipca
```
To check that the remote is added, check that it appears when you do: `git remote -v`. If it is, you can sync your fork with the main fork by pulling:
```bash
git pull fred main
```
To avoid getting out of sync, remember to do this before you start making changes, for example at the beginning of the day.

3. *Use feature branches*: an easy way to keep things organized is to create a new branch when you start working on a new feature/idea/part of the project. Once you are done you can make a pull request to the main branch of the main fork and delete your local/temporary branch once it has been merged. Checking out back to your local main branch and pulling from the newly merged main branch of the main fork will update you nicely and the circle can start again. Here is a small example of how to do this:
```bash
git pull fred main
git checkout -B my_new_branch
... do work ...
git push origin my_new_branch
... make that pull request ...
git checkout main
```
