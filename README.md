# SDK for Cloudflare Workers

This beta package (unstable) includes several tools we found useful while developing on the Cloudflare Developer platform.

---

> [!WARNING]  
> **Archived Repository**  
> This repository is no longer actively maintained and may be removed in the future. As we transition our most complex workflows to more flexible hosting solutions, we have migrated the following core services away from Cloudflare Workers®:  
> - **Authentication**  
> - **File Uploads** (we still recommend checking out [Cloudflare R2](https://www.cloudflare.com/products/r2/) for storage — *we have no financial incentive in suggesting R2 in this document*)  
> - **Database Operations**, due to the exponential growth in demands for our latest applications  
> - **Video Management**, where Cloudflare was only used for storage, not encoding
> - **Link Shortening**, which we no longer provide to direct users, only through automated APIs that trigger when a supported application is used
>  
> Additionally, the name `cfworkers-sdk` became misleading as the project evolved, incorporating utilities that extended beyond the Workers® platform. Implementing these utilities also required advanced knowledge, making the SDK less accessible to the broader community.  
>  
> The associated NPM package, `@homeapis/cfworkers-sdk`, is currently available but may also be removed without notice. We recommend migrating to alternative solutions if you rely on this package.
---

It includes code to reduce time to ship for the following edge computing services:
- A link shortening tool
- URL-based Image storage with Cloudflare R2
- Marketing tools like email collection with D1 (please, review applicable laws in your jurisdiction before storing personal user data)

It requires (for complete feature set only, lightweight mode coming in next months):
* The [itty-router](https://github.com/kwhitley/itty-router) package
* a Cloudflare Account
* Cloudflare Workers enabled on your account
* a Cloudflare D1 database on your account
* a Cloudflare R2 storage bucket on your account

## Installation

* NPM Registry:
```
# install from the NPM registry
npm i @homeapis/cfworkers-sdk
```

* Github Releases:
```
# install from the NPM registry
npm i @homeapis/cfworkers-sdk
```

# Documentation
We provide **experimental** documentation for the project on [homeapis.github.io/cfworkers-sdk](https://homeapis.github.io/cfworkers-sdk/).

## Roadmap
We plan on supporting more Workers features in the coming months.

## Credits
This repository is based on the incredible:
* [itty-router](https://github.com/kwhitley/itty-router) project from @kwhitley
* [@tsndr/cloudflare-workers-jwt](https://www.npmjs.com/package/@tsndr/cloudflare-worker-jwt)

## Legal Notice
We provide this package under the terms of the [MIT license](./LICENSE.MD), allowing you to contribute, distribute, copy, remix and re-use this project as freely as need be.

**We are not affiliated to, or endorsed by Cloudflare, nor the Cloudflare Workers® family of products in any manner.**
