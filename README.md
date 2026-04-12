# gf-p4tterns

Patterns with a refined and expanded parameter set for [gf](https://github.com/tomnomnom/gf), a wrapper around `grep` by [TomNomNom](https://github.com/tomnomnom). These patterns help narrow down large URL lists by matching common query parameters.

## 🛠 Installation

1. Install [gf](https://github.com/tomnomnom/gf) if it is not already installed on your system:
   ```bash
   go install github.com/tomnomnom/gf@latest
   ```
   
2. Clone this repository:
      ```bash
   git clone https://github.com/Danzry/gf-p4tterns.git
   ```

4. Create the `~/.gf` directory, then copy the pattern files into it:
   ```bash
   mkdir -p ~/.gf
   cp gf-p4tterns/*.json ~/.gf
   ```

## ⌨ Usage

1. List all available patterns:
  ```bash
  gf -list
  ```

2. Display only the entries that match the chosen pattern:
  ```bash
  cat urls.txt | gf rce
  ```

## 🗒 Available Patterns

| Pattern | Description |
|---------|-------------|
| `all` | Matches URLs containing query string parameters. |
| `rce` | Matches parameters related to remote code execution. |
| `sqli` | Matches parameters related to SQL injection. |
| `lfi` | Matches parameters related to local file inclusion. |
| `ssti` | Matches parameters related to server-side template injection. |
| `idor` | Matches parameters related to IDOR. |
