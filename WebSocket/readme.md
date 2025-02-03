# Websocket Information
Further testing and documentation necessary

## Base URL
```
wss://api.hyperliquid.xyz/ws
```
<br></br>

# Subscription Requests
<br></br>

## userFills
```
{"method":"subscribe","subscription":{"type":"userFills","user":"id_here","aggregateByTime":true}}
```

## userNonFundingLedgerUpdates
```
{"method":"subscribe","subscription":{"type":"userNonFundingLedgerUpdates","user":"id_here"}}
```
<br></br>

# Responses
<br></br>
## subscriptionResponse
```
{"channel":"subscriptionResponse","data":{"method":"subscribe","subscription":{"type":"userFills","user":"id_here","aggregateByTime":true}}}
```

## userFills
```
{"channel":"userFills","data":{"isSnapshot":true,"user":"id_here","fills":[]}}
```

## userNonFundingLedgerUpdates
```
{"channel":"userNonFundingLedgerUpdates","data":{"isSnapshot":true,"user":"id_here","nonFundingLedgerUpdates":[]}}
```