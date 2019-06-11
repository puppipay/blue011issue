# blue011issue

Example of creating DASH revertible-address. This address is protected by "Locking-Message and PIN"


## How to use this

- Create DASH revertible-address
- Deposit funds you want to send into DASH revertible-address
- Send "Locking-Message and PIN" to the person, you intend go give funds.
- He can withdraw funds using "Locking-Message and PIN"

In case the user does not withdraw or you intend to cancel payment
- You can use the "Locking-Message and PIN" to withdraw the funds your self.

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
# Images of steps

## Download issue script and create DASH revertible-address

<img src="workingimages/issuegetaddress.png" alt="alt text" width="400">

## Load the DASH revertible-address with DASH testcoins

<img src="workingimages/requestdash.png" alt="alt text" width="400">

## Confirm the DASH testcoins is sent

<img src="workingimages/seesent.png" alt="alt text" width="400">


## Verify the DASH revertible-address has received.

By checking balance

<img src="workingimages/seebalance.png" alt="alt text" width="400">

## Now you can send the Locking-message and PIN to other party to receive fund.

In above images

The Locking-message is 
 ``` bash
 
 "message":  "eyJjcmMiOiIyMGUwNjEiLCJ1aWQiOiIwMjEyOGM1OTAzMDNkMTMwZTFmZWMxZWQyNDUzMjE3MGE5OThkOGIxNGYyZWNjNDRiOWY5OTE4MjIyMWVhZGM0MjQiLCJwaW5kYXRhIjp7ImlkIjoiVEVTMTU1NTc1Nzg5NTE2NiIsImRhdGUiOiIxNTYwMjIwNDgyMjIxIiwicGluIjoiIn19"
 
 ``` 
 
 The PIN to unlock is
 ``` bash
 
  "pin": "PIN_6HGPPNB21",
  
  ``` 
  
  The DASH revertible-address having fund is
 
 ``` bash
 
 "address": "92wN1HFM2qmarbxwN25EeeTC4iiF1dZzcx",
  
``` 



