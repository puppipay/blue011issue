# blue011issue

Example of creating revertible DASH address. This address is protected by Locking "Message and PIN"


## How to use this

- Create revertible DASH address
- Deposit funds you want to send into revertible DASH address
- Send locking "Message and PIN" to the person, you intend go give funds.
- He can withdraw funds using "Message and PIN"

In case the user does not withdraw or you intend to cancel payment
- You can use the "Message and PIN" to withdraw the funds your self.

## The sample to withdraw is provided in

https://github.com/puppipay/blue011consume


This example uses testnet.

To get access to use this. Contact puppipay team (puppipay01@gmail.com).

## Content of ./blue011ssuemessage1.sh

``` bash
curl -X POST -H "Authorization: ApiKey eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjVjZWNhYTUzOWRhYzRiNDhkYWQxMzZlNyIsImlhdCI6MTU1OTAxMzk3OX0.hGuhvHO5VWUbExMUnHk5wSKUN27trb2mijxhsYc9Aig" \
 -d @blue011issuemessage1.txt \
 https://dashrevert.belavaditech.com/blue011/issuemessage

```
~                                                        


## Content of ./blue011issuemessage1.txt

The below indicates, message type is default and testnet address is needed.

``` bash

msgtype=default&&network=testnet


```

## Output of command execution of ./blue011issuemessage1.sh

The address created in below output is revertible DASH address. This is protected by "Message and PIN" in that output.

``` bash
./blue011issuemessage1.sh

{
"message":
"eyJjcmMiOiI1YmE0OTgiLCJ1aWQiOiIwMjdjOTg5YTBmOTdkMGFiZjE4MTE4ZjNhZmRjMjJkN2VkNDJhOThiY2MyMWU1ZDRlZjljN2NiNzhmMTczM
DBjOTYiLCJwaW5kYXRhIjp7ImlkIjoiVEVTMTU1NTc1Nzg5NTE2NiIsImRhdGUiOiIxNTU5MTE5ODk2NDkxIiwicGluIjoiIn19",
"pin": "PIN_4PENW2EQ3",
"address": "8pUwBaHuj76YYg5aLHRU3f2XnaPnoiHj6n",
"network": "testnet",
"type": "BLUE011",
}


```


## To check balance in address use below

https://testnet-insight.dashevo.org/insight-api/addr/8pUwBaHuj76YYg5aLHRU3f2XnaPnoiHj6n

``` bash
{"addrStr":"8pUwBaHuj76YYg5aLHRU3f2XnaPnoiHj6n","balance":0,"balanceSat":0,"totalReceived":0,"totalReceivedSat":0,"totalSent":0,"totalSentSa
t":0,"unconfirmedBalance":0,"unconfirmedBalanceSat":0,"unconfirmedTxApperances":0,"unconfirmedAppearances":0,"txApperances":0,"txAppearan
ces":0,"transactions":[]}

```


## Testnet resources

## Loading DASH address with testcoins

It can be loaded from one of the link below

http://test.faucet.masternode.io/
http://faucet.test.dash.crowdnode.io/

## Verifying testnet transaction in blockchain

The transactions reported can be verified using following links

https://testnet-insight.dashevo.org/insight/
http://insight.test.dash.crowdnode.io/
