# Bandersnatch Project

### OS Specific Notes: Gunicorn is not Windows compatible!
- Windows users should not use the `run.sh` shell script, as it depends on gunicorn.
- Windows users should use `py -m app.main` to start the app with Flask acting as the server.
- Windows users may need to download the [wheel for fortuna](https://github.com/decagondev/fortuna-bin-win64) dependency. and follow its [README](https://github.com/decagondev/fortuna-bin-win64/blob/main/README.md)
- Mac and Linux users can use `./run.sh` script or type the command directly `python3 -m gunicorn app.main:APP`.
- Feel free to modify the shell scripts to suit your needs, these are intended to run locally.
- In any case you should not modify the Procfile, this is the run script for the remote server.

  **Working Solution for Windows / Mac / Linux**
