# audio-exp

## Bootstrap

1. Install `rye`
    - following instructions in https://rye-up.com/guide/installation/#installing-rye to install `rye`
      - use `python` provisioned by the `rye`
2. Run `rye sync` to install all specified depedencies and create the virtualenv
    - this should install `maturin` as a development dep for this project and enable compilation of rust code as a python extension
3. Develop in the Rust world
    - run `cargo add <dep>` to install cargo dependencies
    - run `maturin develop --skip-install` to compile rust code to a python extension and make it available in the virtualenv
    - run `rye build` to build wheel
