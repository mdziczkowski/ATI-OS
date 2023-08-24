# ATI-OS

Minimalistic and secure operating system

**Licensing**: See the [LICENSE file](LICENSE.md)

# Features:

## I. Preparation scripts (**Linux only**)

- Small size
- Automation of the most processess related with getting, preparing, compiling and configuration

## II. Final product (Linux disribution):

1. Minimal core - The system base (core) itself contain only files required to start-up and run the system
2. Enchanced security - The system will be defaultly hardened and isolated to provide maximal possible protection. The hardenings include among others:

- kernel hardening
- minimal permissons for the core components of the system
- total isolation from "outside world" (all connections will be done thru secure tunnels)
- installed and configured security software
- multiple security layers

3. Small footprint - In oposite to other Linux distributions, except the security software, there won't be neither a GUI, nor other software preinstalled
4. Full customization - The administrators may freely customize the system (by install the GUI and software at choice) according to the needs

# Requirments:

## Scripts:

1. 64-bit Debian based Linux distribution
2. Pre-Requirments for the build environment - packages and libraries

- build-essentials (install's allmost all software required for the compilation process)
- bison++
- python3
- libraries: libssl-dev
- squashfs
- dependencies required by the third-patry software required to compile the sources

## Final product (portable (live) version)

[!IMPORTANT]
1. USB stick **need to meet** following criteria:

- must be cleaned using the `wipe` command to prevent any potential leftovers from previous data and potential malware
- must have a GPT partition table
- the partition `need` to be set bootable**

2. The BIOS/UEFI `need` to be set to run from USB before the hard drive

3. Ensure yourself to have an active and stable internet connection

4. Ensure yourself that you have fullfilled the requirments of having 

# Distribution preparation using included scripts

1. Get the content of the repository:
  a) using git clone (remember to use the `--recrusive` and `--recrusive-modules` options) OR
  b) Download (and extract the archive)

From now, the folder to with the repository got clobed/extracted will be refered as the "*project dir*"

2. In the `project dir` enter the `code` sub-folder
3. ensure that the scripts are executable
4. run the `prepare.sh` script
5. After the script finishes (assuming that it wasn't interrupted due an error), return to the `project dir` and then enter the `dist` sub-folder
6. copy only the content of the `dist` folder, without copying the folder itself (else the dist won't start)

The distro should be ready to be run.

**IMPORTANT**

The distro has only a console, so you need to be familiar with
