# pythoneda-sandbox/removeme

test domain

## How to declare it in your flake

Check the latest tag of this repository: https://github.com/pythoneda-sandbox-def/removeme, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-sandbox-removeme = {
      [optional follows]
      url =
        "github:pythoneda-sandbox-def/removeme/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [https://nixos/nixpkgs](nixpkgs "nixpkgs") and [https://github.com/numtide/flake-utils](flake-utils "flake-utils").

The Nix flake is managed by the [https://github.com/pythoneda-sandbox-def/removeme](removeme "removeme") definition repository.

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-sandbox-removeme-python38`
- `#packages.[system].pythoneda-sandbox-removeme-python39`
- `#packages.[system].pythoneda-sandbox-removeme-python310`
- `#packages.[system].pythoneda-sandbox-removeme-python311`
