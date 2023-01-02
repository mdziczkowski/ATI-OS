# ATI-OS

Minimalistic and secure operating system

**Licensing**: See the [LICENSE file](LICENSE)

# Features:

## I. Preparation scripts

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
2. Developer environment with following:

- build-essentials (install's allmost all software required for the compilation process)
- bison++
- libraries: libssl-dev
