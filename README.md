Elixir on Alpine Linux
=====

Elixir is a dynamic, functional language designed for building scalable and maintainable applications.

Latest version: **1.2.1**  
Image size: **28.9 MB**  
Parent: [pmbauer/erlang](https://github.com/pmbauer/alpine-erlang)

This is based on work for `msaraiva/erlang` but includes an init system for PID 1 and DNS fixes for Alpine's lack of support for `search` in `resolv.conf`.

See [Erlang/Elixir on Alpine Linux](https://github.com/msaraiva/alpine-erlang) to learn more about creating **minimal Erlang/Elixir docker images with Alpine Linux**.

> **Notice:** This image does not contain git, wget, rebar or hex. If you need to download dependencies, see [pmbauer/elixir-dev](https://registry.hub.docker.com/u/pmbauer/elixir-dev/)

The following packages are pre-installed:

- erlang + dependencies
- elixir

> **Notice:** In order to keep images as compact as possible, Erlang libraries for Alpine Linux are split into many different packages. The full list of Erlang packages available can be found [here](https://pkgs.alpinelinux.org/packages?name=erlang%25&repo=all&arch=x86_64&maintainer=all)

## Usage

```
$ docker run --rm -it pmbauer/elixir iex
Erlang/OTP 18 [erts-7.1] [source] [64-bit] [async-threads:10] [kernel-poll:false]

Interactive Elixir (1.2.1) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)> IO.puts "Hello there!"
Hello there!
:ok
iex(2)>
```
