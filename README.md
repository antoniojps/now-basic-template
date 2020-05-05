# Basic Now CLI API

Bootstrap a serveless typescript API project to deploy at now.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

- Node
- Now CLI

### Installing

1. Clone

```
git clone https://github.com/antoniojps/now-simple-template.git
cd now-simple-template
```

2. Start developing

```
now
now dev
```

Your functions are now running at `http://localhost:3000/api/hello.ts`!

## Deployment

To understand how to deploy read the Now CLI documentation: [Node.js](https://vercel.com/docs/v2/introduction).

```
now --target production
```

## Configuration

The base configuration is at `now.json`, it instructs now to build all the files within the api folder with `@now/node`.

```json
{
  "builds": [{ "src": "api/**/*.[tj]s", "use": "@now/node" }]
}
```

## Authors

- **António Santos** - [antoniosantos.me](https://antoniosantos.me)
