# multi-mono-repo

## Description
This is a sample multi mono repo project that follows all best practices.

## Clone the Repository with Submodules
To clone this repository along with its submodules, use the following command:

```sh
git clone --recurse-submodules <repository-url>
```

If you have already cloned the repository without submodules, you can initialize and update the submodules with:

```sh
git submodule update --init --recursive
```

## Run install_hooks.sh after cloning
The `install_hooks.sh` script copies the hooks from the `hooks` directory to the `.git/hooks` directory and makes them executable.

```sh
chmod +x install_hooks.sh && ./install_hooks.sh
```

## Pre-commit Hook
The pre-commit hook ensures that commit messages follow the Conventional Commits format. If a commit message does not match the required format, the commit will be rejected with an error message.