# Confusing HLS with parent hie.yaml files

To reproduce:

- Navigate to `./foo`
- Run `haskell-language-server`
- Observe that it checks `foo` correctly with the `foo/hie.yaml` cradle
- Run vscode in `foo` and open `Foo.hs`
- Observe that it fails because it tries to read the invalid hie.yaml file in the root directory

This also happens in nvim+coc
