---
layout: single
title:  "Rain Protocol: The Graph Examples"
date:   2022-01-28 15:00:23 +0000
categories: development
---

## GraphQL

As mentioned in our previous article, The Rain Protocol is no exception when it comes to needing data to be indexed, and the team have therefore built out a [Subgraph][subgraph] using [The Graph][the-graph] in order to make retrieval of meaningful information quick and easy. If you don't quite get why indexing is important, check out the [previous article][graph-overview] which gives an overview of the Graph.

Querying a Subgraph involves using a query language called [GraphQL][graph-ql]; this language is not specific to The Graph protocol, and is not even specific to Blockchain based systems. When writing GraphQL, a developer will specify the exact data required in a JSON-like format. A basic example could be querying for: `{ platform { name } }` which would return: `{ "platform": { "name": "Rain Protocol" } }`.

## Examples using Rain Subgraph

The 'Playground' tab under the [Subgraph Explorer][subgraph] can be used to let developers experiment with available data and queries via an easy to use gui. This can also be done easily using an API tool such as [Postman][postman]. To use this, queries should be put into the 'Body', the Method set to `POST`, and then GraphQL selected:


![Seed Phase](https://assets.unegma.net/rainprotocol.xyz/blog/postman-example.jpg "Seed Phase")




[graph-overview]: https://blog.rainprotocol.xyz/various/rain-protocol-the-graph-overview/
[the-graph]: https://thegraph.com/en/
[graph-ql]: https://graphql.org/
[subgraph]: https://thegraph.com/docs/en/developer/define-subgraph-hosted/
[rain-subgraph]: https://thegraph.com/hosted-service/subgraph/beehive-innovation/rain-protocol
[discord]: https://discord.gg/dzYS3JSwDP
[postman]: https://www.postman.com/
