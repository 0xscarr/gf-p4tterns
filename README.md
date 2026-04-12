# gf-p4tterns

gf patterns for [gf](https://github.com/tomnomnom/gf).

These patterns help narrow down large URL lists by matching common query parameters.

> [!NOTE]
> They are meant to support manual review and testing, not to confirm vulnerabilities.

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

- List all available patterns:
  ```bash
  gf -list
  ```

- Read a list of URLs and display only the entries that match the chosen pattern:
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
