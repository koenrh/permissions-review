# permissions.review

[permissions.review](https://www.permissions.review/) is a little guide and checklist that helps you review permissions granted to third-party apps that have access your accounts. Reviewing these permissions, and revoking permissions of apps you don't recognise or don't use, on a regular basis, improves the security of your accounts.

Inspired by incidents such as the [compromise of The Counter](https://techcrunch.com/2017/03/15/twitter-counter-hacked/).

## Contributing

### Adding a site

You can add a site by adding a new entry to the [sites.yml](_data/sites.yml) data file.

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
