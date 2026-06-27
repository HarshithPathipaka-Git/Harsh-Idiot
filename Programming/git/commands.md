
# Installation & Configuration Commands

## Check Git Installation

### Check Git version

```bash
git --version
```

**Use:** Verify that Git is installed and check its version.

---

## Configure Git Identity

### Set username (global)

```bash
git config --global user.name "Your Name"
```

**Use:** Sets your name for all future commits.

---

### Set email (global)

```bash
git config --global user.email "you@example.com"
```

**Use:** Sets the email used for all future commits.

---

### Set default branch

```bash
git config --global init.defaultBranch main
```

**Use:** Makes `main` the default branch when creating new repositories.

---

### Set VS Code as default editor

```bash
git config --global core.editor "code --wait"
```

**Use:** Opens VS Code whenever Git needs an editor.

---

## View Configuration

### View all settings

```bash
git config --list
```

**Use:** Shows every Git configuration currently applied.

---

### View global settings

```bash
git config --global --list
```

**Use:** Displays only your global Git settings.

---

### View username

```bash
git config user.name
```

**Use:** Displays the current username.

---

### View email

```bash
git config user.email
```

**Use:** Displays the current email.

---

## Update Configuration

### Change username

```bash
git config --global user.name "New Name"
```

**Use:** Updates your Git username.

---

### Change email

```bash
git config --global user.email "new@example.com"
```

**Use:** Updates your Git email.

---

## Remove Configuration

### Remove username

```bash
git config --global --unset user.name
```

**Use:** Deletes the configured username.

---

### Remove email

```bash
git config --global --unset user.email
```

**Use:** Deletes the configured email.

---

## Open Git Configuration

### Open global configuration file

```bash
git config --global --edit
```

**Use:** Opens your global `.gitconfig` file for manual editing.

---

### Open local repository configuration

```bash
git config --local --edit
```

**Use:** Opens the current repository's `.git/config` file.

---

## Helpful Commands

### Show where a setting comes from

```bash
git config --show-origin --list
```

**Use:** Shows each configuration value along with the file it was loaded from.

---

### Get a specific setting

```bash
git config --get user.name
```

**Use:** Returns only the configured username.

```bash
git config --get user.email
```

**Use:** Returns only the configured email.