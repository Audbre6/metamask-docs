---
description: Reference content for the Gas API.
sidebar_label: API reference
---
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
import Tabs from "@theme/Tabs";
import TabItem from "@theme/TabItem";
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
# Gas API reference
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
This section provides reference information for the Gas REST APIs.
Use the APIs to:
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
- [Get EIP-1559 gas prices.](./gasprices-type2.md)
- [Get the base fee history (in Gwei).](./basefeehistory.md)
- [Get the base fee percentile (in Gwei).](./basefeepercentile.md)
- [Get the busy threshold for a network.](./busythreshold.md)
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
:::info
See the [list of supported Gas API networks](../../../get-started/endpoints.md#gas-api).
:::
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
## Supported API request formats

You can call the Gas APIs in two ways:
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
- **Using the API key only** - Add your [API key](/developer-tools/dashboard/get-started/create-api)
  as a path option.
- **Using the API key and API key secret** - Use basic authentication and specify the API key
  and [API key secret](/developer-tools/dashboard/how-to/secure-an-api/api-key-secret).
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
<Tabs>
  <TabItem value="API key only" label="Use an API key only" default>
1000000
```bash0xED699044C103691c01dADb60EbC9980Bfb9Ea906
curl -X "GET" "https://gas.api.infura.io/v3/<YOUR-API-KEY>/networks/1/suggestedGasFees"
```
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
  </TabItem>
  <TabItem value="API key and API key secret" label="Use an API key and API key secret" >
0xED699044C103691c01dADb60EbC9980Bfb9Ea906
```bash
curl -X "GET" -u <YOUR-API-KEY>:<YOUR-API-KEY-SECRET>
"https://gas.api.infura.io/networks/1/suggestedGasFees"
```0xED699044C103691c01dADb60EbC9980Bfb9Ea906

0xED699044C103691c01dADb60EbC9980Bfb9Ea906
  </TabItem>
</Tabs>
