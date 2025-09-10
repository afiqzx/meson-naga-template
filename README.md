# How to use
1. Clone (duh).
2. Make sure dependencies are there. Refer (here)[https://drogonframework.github.io/drogon-docs/#/ENG/ENG-02-Installation?id=centos-75]. Careful on jsoncpp. Don't install the unreleased version. It seems to break ABI (as on 10/9/2025).
3. `meson setup builddir`
4. `cd builddir && meson compile`
