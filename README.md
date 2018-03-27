# Veil

![Veil Logo](https://www.veil-framework.com/wp-content/uploads/2013/12/cropped-Veil-Symbol2.png "Veil Logo")

Veil is a tool designed to generate metasploit payloads that bypass common anti-virus solutions.

Veil is current under support by @ChrisTruncer

- - -
## Software Requirements:

The following OSs are officially supported:

- Arch Linux
- BlackArch Linux
- Debian +8
- Deepin +15
- Elementary
- Fedora +22
- Kali Linux Rolling
- Linux Mint
- Parrot Security
- Ubuntu +15.10

## Setup

### Kali's Quick Install

```bash
apt -y install veil
/usr/share/veil/setup/setup.sh -f -s
```

### Git's Quick Install

**NOTE**:
- Installation must be done with superuser privileges. If you are not using the root account (as default with Kali Linux), prepend commands with `sudo` or change to the root user before beginning.
- Your package manager may be different to `apt`.

```bash
sudo apt-get -y install git
git clone https://github.com/Veil-Framework/Veil.git
cd Veil/
sudo ./setup/setup.sh -f -s
```

### Py2Exe

**NOTE**: Using **Py2Exe** is recommended over Pyinstaller _(as it has a lower detection rate)_.

Install on a Windows Computer:

- [Python 3.3](https://www.python.org/downloads/release/python-335/)
- [Py2Exe](https://pypi.python.org/pypi/py2exe/)
- [PyCrypto](http://www.voidspace.org.uk/python/modules.shtml#pycrypto)
- [PyWin32](https://sourceforge.net/projects/pywin32/files/pywin32/Build%20221/)

### Regenerating Configuration file

Most of the time the config file at `/etc/veil/settings.py` will not need to be rebuilt but in some cases you might be prompted to do so. The file is generated by `./config/update.py`.

It is important that you are in the `config`/ directory before executing update.py. If you are not, settings.py will be incorrect and when you launch Veil you will see the following.

```bash
    Main Menu

            0 payloads loaded
```

Don't panic. Enter the `./config/` directory and re-run `./update.py`.

- - -

## Licensing

This project is licensed under the GNU General Public License v3 license.
