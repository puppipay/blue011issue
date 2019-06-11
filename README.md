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

``` bash
It can be loaded from one of the link below


http://test.faucet.masternode.io/
http://faucet.test.dash.crowdnode.io/

```

## Verifying DASH testnet address has balance 

``` bash
In below link replace the address with your DASH testnet address 

https://testnet-insight.dashevo.org/insight-api/addr/92wN1HFM2qmarbxwN25EeeTC4iiF1dZzcx


```


![Image description](workingimages/requestdash.png =400x400)

<img src="workingimages/requestdash.png" alt="alt text" width="400" height="400">

