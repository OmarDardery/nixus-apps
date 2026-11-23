# Apps

Managed by Nixus. One folder per app:

- `compose.yaml` and build files: the app (images pinned by digest).
- `default.nix`: optional Nix declaration (VMs, containers, options).
- `secrets.enc.yaml`: environment variables, encrypted with SOPS to the
  server's age key. Edit them in the console's Env tab.

Push changes here and review them in the console under Backups → Apps repository.
Never commit plaintext secrets or private keys.
