# Feature Flag Solutions

## What are Feature Flags?

`Feature Flags` are a technique in software development that allows to modify runtime behavior without changing code. It decouples the releasing of functionality to the end users from the roll-out of the binaries.
`Feature Flags` work like a switch or toggle and are therefore often called `Feature Toggles` or `Feature Switches` because of there Boolean nature. But `Feature Flags` can have many different use cases and can be more complex than a toggle. That’s why the tern Feature Flag is more suitable.

## Available Feature Flag Solutions

There are many solutions out there. I'm first focusing on all the available `products` - and not on individual frammeworks. Maybe I add this later. This is the criteria I will look for:

- Pricing
- License
- Available SDKs
- Hosting Options
- Compliance

These are the solutions I found so far. Feel free to contact ne if I missed anything:

1. [LaunchDarkley](#launchdarkley)
2. [Unleash](#unleash)
3. [Switchover](#switchover)
4. [VWO](#vwo)
5. [Split](#split)
6. [Flagship](#flagship)

## LaunchDarkley

[LaunchDarkley](https://launchdarkly.com) is one of the oldest players in the field of Feature Flags and a very mature solution with the most SDKs and certifications available.

### LaunchDarkley Pricing

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

### LaunchDarkley Available SDKs (26)

|               |                |                |               |
|---------------|----------------|----------------|---------------|
| Android       | Apex           | C/C++**        | C#            |
| Electron      | Erlang         | Flutter        | Gatsby        |
| Go            | Haskell        | iOS            | Java          |
| JavaScript    | Lua            | .NET           | Node.JS**     |
| PHP           | Python         | React          | React Native  |
| Roku          | Ruby           | Swift          | Xamarin       |

`**`client and server

### LaunchDarkley Hosting options

LaunchDarkly is a SaaS service. But at least a few years ago it was possible to install it on-premises if
you asked for an enterprise plan. I have to validate if this is still the case.

### LaunchDarkley Compliance

- SOC 2 Type II
- ISO 27001
- GDPR
- EU/US Privacy Shield

## Unleash

[Unleash](https://www.getunleash.io/) is a product that has an [Open Core](https://github.com/Unleash/unleash) but is also offered as a SaaS service. Unleash is the solution that is used by GitLab.

### Unleash Pricing

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

### Unleash Hosting options

Self-hosted or SaaS

### Unleash Available SDKs (11)

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

### Unleash Compliance

Self-hosted: you have full control.
Service: unknown

## Switchover

[Switchover](https://switchover.io/) is a product of the German company Takso GmbH with a strong focus on compliance in the automotive industry.

### Switchover Pricing

|                     | Free.              | Starter            | Professional       | Enterprise         |
| --------------------|-------------------:|-------------------:|-------------------:|-------------------:|
| Price / month       |              0 EUR |             39 EUR |             89 EUR |            199 EUR |
| Seats               |                  1 |                  5 |                 50 |          unlimited |
| Requests            |              5 mio |             15 mio |             90 mio |          unlimited |
| Projects            |                  1 |                  3 |                 10 |          unlimited |
| SLA                 |                98% |              98.5% |              99.5% |              99.5% |

### Switchover Hosting options

SaaS.
I had contact with Switchover and they said they support self hosting. But I can't find anything on the website.

### Switchover Available SDKs (8)

- PHP
- Laravel
- Node.JS
- JavaScript
- React
- Vue JS
- Angular JS
- Nuxt JS

### Switchover Compliance

unknown (probably through self hosting)

## VWO

[VWO](https://vwo.com/) is mkore than just Feature Flags - they provide analytics and testing solutions and services. Unfortunatley they don't have apricing on their website. I'll skipp them therefor for now.

## Split

[Split](https://www.split.io/) is a feature feature management and experimentation platform that pairs feature flagging with data to automatically attribute system performance and user behavior to each feature. They serve over 1 trillion flags per month according to their website. Split is headquartered in Redwood City, California.

### Split Pricing

Split has four pricing tiers, starting with a free-forever Developer tier. Beyond the Developer tier, pricing is based primarily on seats, with additional costs if monthly tracked keys (MTKs) exceed 50,000. One MTK = one unique user or account or device evaluated by SDK. Developer tier accounts begin with a 30-day Enterprise trial. See summary below and details on [their website](https://www.split.io/pricing/).

|                     | Developer          | Team               | Business             | Enterprise           |
| --------------------|-------------------:|-------------------:|---------------------:|---------------------:|
| Price/seat/month.   |                $ 0 |               $ 33 |                 $ 60 |               Custom |
| Max Feature Flags   |          Unlimited |          Unlimited |            Unlimited |            Unlimited |
| Max Workspaces      |                  1 |                  1 |            Unlimited |            Unlimited |
| Max Environments    |                  2 |                  2 |            Unlimited |            Unlimited |
| Treatments per flag |                  2 |                  2 |            Unlimited |            Unlimited |
| SLA                 |                  - |              99.9% |                99.9% |                99.9% |
| Standard MTKs       |             50,000 |             50,000 |               50,000 |               50,000 |
| Additional MTKs     |      Not available |      Not available |               Custom |               Custom |

### Split Available SDKs (16 + Evaluator)

- Angular
- Android
- Flutter
- Go
- iOS
- Java
- JavaScript
- .NET
- Node.JS
- PHP
- Python
- React
- React Native
- Redux
- Ruby
- Ruby on Rails
- Split Evaluator to support other languages via REST API

### Split Hosting Options

SaaS only.
Split provides an on-premise [Split Proxy](https://help.split.io/hc/en-us/articles/4415960499213-Split-Proxy) if limiting outbound traffic to a single connection is desired

### Split Compliance

Split is CCPA, GDPR, ISO 20001, Privacy Shield and SOC 2 certified.
More detail and access to pentest reports, etc is available on the [Split Security Portal](https://security.split.io/)

## Flagship

[Flagship](https://www.flagship.io/) is a French company with headquaters in Paris and offices around the world (New York, San Francisco, London, Singapore, Berlin, Cologne, Madrid).

### Flagship Pricing

[Pricing](https://www.flagship.io/pricing/)

|                     | Premium            | Enterprise         |
| --------------------|-------------------:|-------------------:|
| Price / month       |               $175 |                  ? |
| Seats               |          unlimited |          unlimited |
| Environments        |                  2 |             Custom |
| Projects / Environment |               2 |          Unlimited |
| MAU`*`              |                15k |               300k |
| SLA                 |                  - |             99.99% |

### Flagship Available SDKs (12)

- JavaScript
- Node.JS
- React
- Go
- Java
- Python
- PHP
- .NET
- Flutter
- iOS
- Android
- React Native

### Flagship Hosting Options

???

### Flagship Compliance

???

## Summary

This analysis is still work in progress. Let me know if you miss anything. Contact me or directly create a pull request.
