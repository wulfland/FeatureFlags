# Feature Flag Solutions

## What are Feature Flags?

`Feature Flags` are a technique in software development that allows to modify runtime behavior without changing code. It decouples the releasing of functionality to the end users from the roll-out of the binaries.
`Feature Flags` work like a switch or toggle and are therefore often called `Feature Toggles` or `Feature Switches` because of there Boolean nature. But `Feature Flags` can have many different use cases and can be more complex than a toggle. That’s why the tern Feature Flag is more suitable.

## Feature Flag Solutions

There are many solutions out there. I'm first focusing on all the available products. This is the criteria I will look for:

- Pricing
- License
- Available SDKs
- Hosting Options
- Compliance

## LaunchDarkley

[LaunchDarkley](https://launchdarkly.com) is one of the oldest players in the field of Feature Flags.

### Pricing

See [Pricing](https://launchdarkly.com/pricing/). LaunchDarkly is purchachsed on a monthly basis but can be payed anualy.

These plans are available:

|                     | Starter            | Pro                | Enterprise         |
| --------------------|-------------------:|-------------------:|-------------------:|
| Price payed monthly:|                $10 |               $20  |                  ? |
| Price payed anualy: |              $8.33 |             $16.67 |                  ? |
| Seats minimum       |                  1 |                  5 |                 25 |
| MAU`*`              |                 1k |                10k |                  ? |
| SSO / SAML          |     $10/seat/month |     $10/seat/month |           included |
| SLA                 |                  ? |              99.9% |              99.9% |

`*`Monthly active unique client-side users

A seat is a team member that logs into the portal using a unique email address.
The MAUs are the active unique users - so every user only counts once - even if they evaluate flags from multiple devices.

### Available SDKs (26):
|               |                |                |               |
|---------------|----------------|----------------|---------------|
| Android       | Apex           | C/C++`**`      | C#            |
| Electron      | Erlang         | Flutter        | Gatsby        |
| Go            | Haskell        |iOS             | Java          |
| JavaScript    | Lua            | .NET           | Node.JS`**`   |
| PHP           | Python         | React          | React Native  |
| Roku          | Ruby           | Swift          |  Xamarin      |

`**`client and server

### Hosting options

LaunchDarkly is a SaaS service. But at least a few years ago it was possible to install it on-premises if
you asked for an enterprise plan. I have to validate if this is still the case.

### Compliance

- SOC 2 Type II
- ISO 27001
- GDPR
- EU/US Privacy Shield

## Unleash

[Unleash](https://www.getunleash.io/) is a product that has an [Open Core](https://github.com/Unleash/unleash) but is also offered as a SaaS service. Unleash is the solution that is used by GitLab.

### Pricing

The open core can be self-hosted using **Docker**, **Node.js**, or **Helm** and is free of charge.

Unleash Enterprise comes with two additional [plans](https://www.getunleash.io/plans#compare): `Pro` and `Enterprise`. Enterprise can be hosted or a self.hosted solution.

|                     |  Pro                | Enterprise         |
| --------------------|--------------------:|-------------------:|
| Price payed monthly:|$16 (first 5 than 15)|                  ? |
| Price payed anualy: |              $16.67 |                  ? |
| Seats min - max     |              5 - 20 |                  ? |
| MAU`*`              |                 ?   |                  ? |
| SLA                 |               99.9% |              99.9% |

`*`Monthly active unique client-side users
`***`host

### Hosting options

Self-hosted or SaaS

### Available SDKs (11)

Official Server SDKs:

- [Java SDK](https://docs.getunleash.io/sdks/java_sdk)
- [Node.js SDK](https://docs.getunleash.io/sdks/node_sdk)
- [Go SDK](https://docs.getunleash.io/sdks/go_sdk)
- [Ruby SDK](https://docs.getunleash.io/sdks/ruby_sdk)
- [Python SDK](https://docs.getunleash.io/sdks/python_sdk)
- [.Net SDK](https://docs.getunleash.io/sdks/dot_net_sdk)
- [PHP SDK](https://docs.getunleash.io/sdks/php_sdk)

Official Frontend SDKs:

The frontend SDKs connects via the [Unleash Proxy](https://docs.getunleash.io/sdks/unleash-proxy) in order to ensure Privacy, scalability and security.

- [Javascript SDK](https://docs.getunleash.io/sdks/proxy-javascript)
- [React SDK](https://docs.getunleash.io/sdks/proxy-react)
- [Android SDK](https://docs.getunleash.io/sdks/android_proxy_sdk)
- [iOS SDK](https://docs.getunleash.io/sdks/proxy-ios)

## Switchover

https://switchover.io/

## VWO

https://vwo.com/

## Split

https://www.split.io/

## Flagship 

https://www.flagship.io/

