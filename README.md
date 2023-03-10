# esp-template

A minimalist template for use with [cargo-generate] to create `no_std` applications targeting Espressif's line of SoCs and modules. At present this template supports the **ESP32**, **ESP32-C2**, **ESP32-C3**, **ESP32-S2**, and **ESP32-S3**; additional devices will be added as they become available.

To generate a project using this template:

```bash
cargo generate -a FMFigueroa/esp-template
```

After running the command, there will be a few prompts:

- `Project Name`: Name of the crate.
- `Which MCU to target?`: SoC model.
- `Enable allocations via the esp-alloc crate?`: Adds [`esp-alloc`] dependency, and initializes the heap.
- `Configure project to use Dev Containers (VS Code, GitHub Codespaces and Gitpod)?`: Adds support for:

  - [VS Code Dev Containers]
  - [GitHub Codespaces]
  - [Gitpod]

  Dev Containers also allow flashing from the container using [web flash] and have integration with [Wokwi simulator] via the [VS Code Wokwi extension](only available in VS Code and GitHub Codespaces).

For a more detailed explanation about the template see [Understanding esp-template] chapter of [The Rust on ESP Book].

[cargo-generate]: https://github.com/cargo-generate/cargo-generate
[`esp-alloc`]: https://github.com/esp-rs/esp-alloc
[vs code dev containers]: https://code.visualstudio.com/docs/remote/containers#_quick-start-open-an-existing-folder-in-a-container
[github codespaces]: https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace
[gitpod]: https://www.gitpod.io
[wokwi simulator]: https://wokwi.com/
[vs code wokwi extension]: https://marketplace.visualstudio.com/items?itemName=wokwi.wokwi-vscode
[web flash]: https://github.com/bjoernQ/esp-web-flash-server
[understanding esp-template]: https://esp-rs.github.io/book/writing-your-own-application/no-std-applications/understanding-esp-template.html
[the rust on esp book]: https://esp-rs.github.io/book/

## License

Licensed under either of:

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in
the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without
any additional terms or conditions.