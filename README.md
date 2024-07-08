# Offsec Wiki

Pentest notes, not intended to be complete ;)

## Installation

```bash
# clone the repository
git clone git@github.com:simonjujuh/offsec-wiki.git /opt/my-resources/wiki

# Create aliases to fetch the offsec wiki
alias wis='f() { cd /opt/my-resources/wiki; batcat -p -l md "$(find . -type f -name "*.md" | fzf)" }; f'
alias wie='f() { cd /opt/my-resources/wiki; vim "$(find . -type f -name "*.md" | fzf)" }; f'
alias wio='subl /opt/my-resources/wiki'
```