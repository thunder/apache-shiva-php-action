# apache-shiva-php-action
This is a GitHub action that runs Apache with mod_php to serve a website. Use after [Setup PHP in GitHub Actions](https://github.com/shivammathur/setup-php).

**Assumes you are using Ubuntu**

## Example usage
<!-- TODO: update -->
```yaml
- name: Setup PHP
  uses: shivammathur/setup-php@v2
  with:
    php-version: '7.4'
- name: Setup Apache
  uses: thunder/apache-shiva-php-action
  with:
    php-version: '7.4'
    site-directory: /path/to/code
    # Defaults to 8888
    http-port: 8080
```