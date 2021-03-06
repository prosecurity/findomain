# Findomain
A tool that use Certificates Transparency logs to find subdomains.

# How it works?
It tool doesn't use the common methods for sub(domains) discover, the tool uses Certificate Transparency logs to find subdomains and it method make it tool very faster and reliable. If you want to know more about Certificate Transparency logs, read https://www.certificate-transparency.org/

# Installation
If you want to install it, you can do that manually compiling the source or using the precompiled binary.

**Manually:**
You need to have [Rust](https://www.rust-lang.org/) installed in your computer first.

```
$ git clone https://github.com/Edu4rdSHL/findomain.git
$ cd findomain
$ cargo build --release
$ sudo cp target/release/findomain /usr/bin/
$ findomain
```

**Using the binary:**

```
$ git clone https://github.com/Edu4rdSHL/findomain.git
$ sudo cp findomain/bin/findomain /usr/bin
$ findomain
```
**If you are using the [BlackArch Linux](https://blackarch.org) distribution, you just need to use:**

```
$ sudo pacman -S findomain
```

# Usage

You can use the tool in two ways, only discovering the domain name or discovering the domain + the IP address.

```
findomain 0.1.2
Eduard Tolosa <tolosaeduard@gmail.com>
A tool that use Certificates Transparency logs to find subdomains.

USAGE:
    findomain [FLAGS] [OPTIONS]

FLAGS:
    -h, --help       Prints help information
    -i, --get-ip     Return the subdomain list with IP address if resolved.
    -V, --version    Prints version information

OPTIONS:
    -f, --file <file>        Sets the input file to use.
    -t, --target <target>    Target host
```
# Demo
<a href="https://asciinema.org/a/gAyQxtZkQ0LO792olEEXUkpCz" target="_blank"><img src="https://asciinema.org/a/gAyQxtZkQ0LO792olEEXUkpCz.svg" /></a>

# Issues and requests
If you have problems or want and enhancement request, open an [issue](https://github.com/Edu4rdSHL/findomain/issues).
