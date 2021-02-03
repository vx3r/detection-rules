## Red Team Automation

[![Supported Python versions](https://img.shields.io/badge/python-3.7+-yellow.svg)](https://www.python.org/downloads/)
[![Chat](https://img.shields.io/badge/chat-%23security--detection--rules-blueviolet)](https://ela.st/slack)

The repo comes with some red team automation ([RTA](./)) python scripts that run on Windows, Mac OS, and \*nix. 
RTA scripts emulate known attacker behaviors and are an easy way too verify that your rules are active and working as expected.

```console
$   python -m rta -h
usage: rta [-h] ttp_name

positional arguments:
  ttp_name

optional arguments:
  -h, --help  show this help message and exit
```
<<<<<<< HEAD
ttp_name can be found in the [rta](./rta) directory. For example to execute `./rta/wevtutil_log_clear.py` script, run command:
=======
`ttp_name` is the name of a script that can be found in the [rta](./rta) directory. For example, to execute ./rta/wevtutil_log_clear.py script, run command:
>>>>>>> 607d8cf06a298ec4edf8c0e326b3c1a9ace509ea

```console
$ python -m rta wevtutil_log_clear
```

Most of the RTA scripts contain a comment with the rule name, in `signal.rule.name`, that maps to the Kibana Detection Signals.