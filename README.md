# oauth2-proxy-hands-on

## Description

This is a hands-on project to learn how to use OAuth2 Proxy with GitHub.

### Containers

- nginx
  Serve static files in `nginx/html`
- oauth2-proxy
  OAuth2 Proxy
- redis
  Session store for OAuth2 Proxy

## Usage

1. Register a new OAuth2 application on GitHub
   [Developer applications](https://github.com/settings/developers)

1. Update `.env` with your secrets

1. Run containers

   ```shell
   docker-compose up
   ```

1. Access [http://localhost](http://localhost)
   With authentication, access [http://localhost](http://localhost).
   If you want to check nginx without authentication, access [http://localhost:8000](http://localhost:8000).

   As you could see from this, nginx port (8000) should be closed externally except for hands-on use.
