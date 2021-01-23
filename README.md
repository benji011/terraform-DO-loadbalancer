# Terraform sandbox

## Description
A personal sandbox for me to better understand [IaC](https://en.wikipedia.org/wiki/Infrastructure_as_code) using [Terraform](https://github.com/hashicorp/terraform) together with [DigitalOcean](https://www.digitalocean.com/) as my provider (over other resources like AWS).

This repo, so far, allows you to provision 2 droplets behind 1 load balancer and gives you a domain (which you can modify yourself to match your own needs)

## About the file structure

All `.tf` files are categorized and stored under directories named after the resources they use (e.g. droplet for droplets). 

```bash
├── README.md
├── domain
│   └── my_domain.tf
├── droplet
│   ├── www-1.tf
│   └── www-2.tf
├── loadbalancer
│   └── loadbalancer.tf
└── provider.tf
```

This doesn't mean they should be stored that way. It's really just a sandbox for me to better understand how Terraform works as a platform. Eventually I want to create a separate repo for an actual Terraform project.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
