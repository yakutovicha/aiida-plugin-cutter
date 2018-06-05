# {{ cookiecutter.plugin_name }}

{{ cookiecutter.short_description }}

# Installation

```shell
git clone https://github.com/{{ cookiecutter.github_user }}/{{ cookiecutter.repo_name}} .
cd {{ cookiecutter.repo_name }}
pip install -e .  # also installs aiida, if missing (but not postgres)
#pip install -e .[precommit,testing] # install extras for more features
verdi quicksetup  # better to set up a new profile
verdi calculation plugins  # should now show your calclulation plugins
```

# Usage

Here goes a complete example of how to submit a test calculation using this plugin.

# License

MIT

# Contact

{{ cookiecutter.contact_email }}