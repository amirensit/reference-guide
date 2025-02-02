# Minor Releases

Any patch release made for an Axon project aims to resolve bugs.
This page provides an overview of patch releases for the Axon Reactor Extension.

## Release 4.4

### Release 4.4.3

* Issues arose when using Spring Boot Dev Tools in combination with the Axon Reactor Extension.
  Contributor `magnusheino` noted this problem in issue [#28](https://github.com/AxonFramework/extension-reactor/issues/28).

* The `ReactorCommandGateway` and `ReactorQueryGateway` introduced a discrepancy compared to Axon Framework.
  Namely, the gateways swallowed exceptions instead of throwing them to the user.
  We resolved this issue in [this](https://github.com/AxonFramework/extension-reactor/pull/18) pull request by unwrapping the exception message into the returned `Mono` or `Flux`

For the complete list of changes, check out [this](https://github.com/AxonFramework/extension-reactor/issues?q=is%3Aclosed+milestone%3A%22Release+4.4.3%22) page.
