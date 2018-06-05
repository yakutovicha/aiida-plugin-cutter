# AiiDA plugin cutter

Cookie cutter recipe for [AiiDA](http://www.aiida.net) plugins.

## Usage

    pip install cookiecutter
    cookiecutter git@github.com:aiidateam/aiida-plugin-cutter.git

![Demo](demo.gif "The fastest way to kickstart an AiiDA plugin.")

This will produce the files and folder structure for your plugin,
already adjusted for the name of your plugin.

## Development

The plugin cutter comes with rather strict continuous integration tests which

 * test that the cookiecutter recipe works
 * test that the plugin can be installed
 * test that the unit test(s) of the plugin run
 * test that the code of the plugin confirms to coding standards

Particularly the last test is very easy to break.
In order to check your syntax, do:
```
cookiecutter --no-input -f .
pip install -e aiida-diff[docs,pre-commit,testing]
cd aiida-diff
git init && git add -A
pre-commit install
pre-commit run
```


## License

MIT

## Contact

Please report issues to the GitHub issue tracker. Other inquiries may be
directed to the [AiiDA mailinglist](http://www.aiida.net/mailing-list/).