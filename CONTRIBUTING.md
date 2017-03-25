# Contributing

## Adding a service

You can add a service by adding a new entry to the [services.yml](_data/services.yml) data file.

Make sure to include the following keys:

- `name` - Name of the service.
- `description` - A few-word description of the service.
- `url` - URL of the main page of the service.
- `review_url` - URL of the page on which permissions can be managed.

Optionally, include a link (using the key `docs_url`) to service's own documentation regarding third-party app permissions.

See, for example, GitHub's entry:

```yaml
- name: GitHub
  description: Hosting service for software development.
  url: https://github.com/
  review_url: https://github.com/settings/applications
  docs_url: https://help.github.com/articles/connecting-with-third-party-applications
```

If possible, include a square icon of the service in the `images/` folder of which the file name should equal the name of the service down-cased (e.g. `github.png` for `GitHub`).
