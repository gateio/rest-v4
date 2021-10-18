# Gate API v4 v4.22.0
Welcome to Gate.io API

APIv4 provides spot, margin and futures trading operations. There are public APIs to retrieve the real-time market statistics, and private APIs which needs authentication to trade on user's behalf.

Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.  
- [Access URL](#Access-URL)  
- [SDK](#SDK)  
- [API Performance](#API-Performance)  
- [Market business application](#Market-business-application)

## Access URL
REST API BaseURL:

- Live trading: https://api.gateio.ws/api/v4
- Futures TestNet trading: https://fx-api-testnet.gateio.ws/api/v4
- Futures live trading alternative (futures only): https://fx-api.gateio.ws/api/v4      


## SDK
Available SDK:

- [Python](https://github.com/gateio/gateapi-python "Python")
- [Java](https://github.com/gateio/gateapi-java "Java")
- [PHP](https://github.com/gateio/gateapi-php "PHP")
- [Go](https://github.com/gateio/gateapi-go "Go")
- [C#](https://github.com/gateio/gateapi-csharp "C#")
- [NodeJS](https://github.com/gateio/gateapi-nodejs "NodeJS")
- [Javascript](https://github.com/gateio/gateapi-js "Javascript")

Besides API examples, some SDK provides an additional demo application. The demo application is a relatively complete example demonstrating how to use the SDK. It can be built and run separately. Refer to corresponding repository for details.

- [Python](https://github.com/gateio/gateapi-python/tree/master/example "Python")
- [Java](https://github.com/gateio/gateapi-java/tree/master/example "Java")
- [C#](https://github.com/gateio/gateapi-csharp/tree/master/example "C#")
- [Go](https://github.com/gateio/gateapi-go/tree/master/_example "Go")

[More >>](https://www.gate.io/docs/developers/apiv4/en/ "More >>")

## API Performance
<table>
    <thead>
        <tr>
            <th>Markets</th>
            <th>Endpoints</th>
            <th>Limits</th>
            <th>Based On</th>
            <th>include</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=4>Spot</td>
            <td >Public endpoints</td>
            <td >900r/s</td>
            <td >API Key</td>
        	  <td > Depth,Kline,trading pairs,etc.</td>
        </tr>
        <tr>
            <td>Private endpoints</td>
            <td rowspan=2>900r/s</td>
            <td rowspan=2>API Key</td>
            <td> Trading history,fee rate,etc.</td>
        </tr>
        <tr>
        	<td>Place orders</td>
        	<td>Placing(bulk)orders,margin trade,etc.
        </tr>
        <tr>
        	<td> Cancel orders</td>
        	<td> 5000r/s </td>
        	<td> API Key </td>
        	<td>Canceling(all)orders,etc.</td>
        </tr>
        <tr>
            <td rowspan=4>Perp Swaps</td>
            <td >Public endpoints</td>
            <td >300r/s</td>
            <td >IP</td>
        	  <td > Depth,Kline,trading pairs,funding rate,etc.</td>
        </tr>
        <tr>
            <td>Private endpoints</td>
            <td rowspan=3>400r/s</td>
            <td rowspan=3>User ID</td>
            <td>Position,fee rate,etc.</td>
        </tr>
        <tr>
        	<td>Place orders</td>
        	<td> Placing(bulk)orders,margin trade,etc.
        </tr>
        <tr>
        	<td> Cancel orders</td>
        	<td> Canceling(all)orders,etc.</td>
        </tr>
    </tbody>
</table>
- The rate limit is counted against each sub-accountor main account.</br> 

Web socket:

- The message limit sent to the server: unlimited.
-  Number of connections per IP: ≤ 300

NOTICE:

When repeatedly violating rate limits, it dependson

- the request< burst rate, the request will have a delay.
- the request> burst rate, the request will be declined.

# Market business application

In order to further improve the market depth and transaction liquidity of the platform, we will recruit institutional market makers in an open and transparent manner, and provide professional market makers with professional market makers based on their contributions to platform liquidity. Rate scheme.

- Provide Gateio UID
- Provide screenshots of his trading volume or VIP level, etc.
- Provide screenshots of his trading volume or VIP level, etc.

Provide the above content and submit it to <b>mm@mail.gate.io</b> , we will accept it within 3 working days.</br>
VIP11 and above need to enable GT deduction in the personal center to enjoy the professional market merchant rate.

