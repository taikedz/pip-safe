# pip-safe

Safely use `pip` command without affecting your host environment by forcing use of a virutalenv.

You can `alias pip=pipsy` in your `.bashrc` to benefit from it.

    pipsy COMMAND [OPTIONS  ...]
 
A molly-guard to prevent running pip in the host environment.
 
Set a default virtual environment for pipsy, and it will be used for any pipsy command.
 
pipsy set VENVNAME
    Set a virtual env name for subsequent pipsy executions.
 
pipsy ls
    List available environments
 
pipsy which
    Print currently defaulted environment
 
The run any pip commands you normally would like
 
pipsy install youtube-dl
    Install the "youtube-dl" pip package
 
Or, the special actions
 
pipsy run COMMAND [ARGUMENTS ...]
    Run a command that was installed in the virtualenv
 
    pipsy run youtube-dl ...
