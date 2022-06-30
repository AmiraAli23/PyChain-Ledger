# PyChain-Ledger

![image](https://user-images.githubusercontent.com/99091066/176038653-1859c89c-e980-4e55-ad7b-d29bed95c018.png)

For this project, we were tasked to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions and to verify the integrity of the data in the ledger.

## Step 1: Create a Record Data Class

Define a new class named Record. Add the @dataclass decorator immediately before the Record class definition.

<img width="99" alt="Screen Shot 2022-06-30 at 6 52 21 PM" src="https://user-images.githubusercontent.com/99091066/176791480-c4a2f63b-823d-405b-96f8-4f612c3bbb1a.png">

Add an attribute named sender of type str, an attribute named receiver of type str, and an attribute named amount of type float.


<img width="108" alt="Screen Shot 2022-06-30 at 6 53 03 PM" src="https://user-images.githubusercontent.com/99091066/176791539-c5d06d1e-6596-4037-bf59-a58361087fbe.png">

The sender/receiever will be names and the amounts will be values. 

## Step 2: Modify the Existing Block Data Class to Store Record Data

In the Block class, rename the data attribute to record.
Set the data type of the record attribute to Record.

<img width="577" alt="Screen Shot 2022-06-30 at 6 57 29 PM" src="https://user-images.githubusercontent.com/99091066/176791963-e2e3be66-414a-4bb0-b802-7d23f739adf0.png">

## Step 3: Add Relevant User Inputs to the Streamlit Interface


<img width="646" alt="Screen Shot 2022-06-30 at 6 59 08 PM" src="https://user-images.githubusercontent.com/99091066/176792176-fbee240d-49d0-43a6-bb4d-c807e8e65cf1.png">

These sender, receiver, and amount lines allow the user to enter in values. The record then consists of the sender, receiver, amount, creator ID, and previous hash.

## Step 4: Test the PyChain Ledger by Storing Records

<img width="1076" alt="Screen Shot 2022-06-30 at 7 04 17 PM" src="https://user-images.githubusercontent.com/99091066/176792658-3f815065-3f5b-4c56-bd82-056251761573.png">

  > Block Difficulty 1 

<img width="1079" alt="Screen Shot 2022-06-30 at 7 05 03 PM" src="https://user-images.githubusercontent.com/99091066/176792735-49de5d2c-ec22-4022-85ca-c878b7cb760b.png">

  > Block Difficulty 2 


<img width="1083" alt="Screen Shot 2022-06-30 at 7 05 44 PM" src="https://user-images.githubusercontent.com/99091066/176792798-a40f380f-dec4-482f-8963-d48793700ded.png">

  > Block Difficulty 5 

<img width="1114" alt="Screen Shot 2022-06-30 at 7 06 21 PM" src="https://user-images.githubusercontent.com/99091066/176792858-ad261535-1b18-4ad0-83f5-e012020a81b0.png">

  > Drop-down menu
  

<img width="622" alt="Screen Shot 2022-06-30 at 7 06 51 PM" src="https://user-images.githubusercontent.com/99091066/176792909-8d3f2d36-c567-48a3-b5e9-c5a38e0418e4.png">
