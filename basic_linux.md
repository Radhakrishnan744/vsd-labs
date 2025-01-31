SKY130 DAY 1

Basic Git hub keywords:

1.cd 'name' = to switch to a different directory

2.ls = to see the directory's contents

3.cd = to come to home directory

![IMG_20250131_230715](https://github.com/user-attachments/assets/93b1147c-d089-4fb6-9291-94061278b52c)
![IMG_20250131_230730](https://github.com/user-attachments/assets/9ea0bd3f-7e97-44be-975e-9f6a44dff7ae)
![IMG_20250131_230735 (1)](https://github.com/user-attachments/assets/02fdac4a-ad64-4c0a-9284-ecc8bedbbce8)
![IMG_20250131_230723](https://github.com/user-attachments/assets/ceeaa083-b368-4f3d-925a-81378ce7d53d)

So, let us move on to open lane

To open this, we have to perform the following steps in the terminal. First, open the Openlane directory and type the below commands
![image](https://github.com/user-attachments/assets/1b1e4a31-c646-46c3-8278-c763a1fdd51c)

Then, we have to prepare the design by typing,

![image](https://github.com/user-attachments/assets/097be3b2-1073-4d93-87ef-9c85d466c230)

Here, the lef files are merged.

Thus, now we can move onto synthesis.

One thing to be noted is that our actions are recorded in the designs -> picorv32a -> runs -> time period
-> tmp

![image](https://github.com/user-attachments/assets/287b0269-2913-4872-baec-109690e3b9ae)

By using the less cmds.logs prompt we get the history,
![image](https://github.com/user-attachments/assets/3b8c6a19-4aee-4378-a73b-77faa8f05702)

So, let move onto synthesis. After, a bit of a wait, we get:
![image](https://github.com/user-attachments/assets/ffba284c-813d-4d2c-bcf2-581cf8033231)

and by checking in the runs, sure enough, we find synthesis.

![image](https://github.com/user-attachments/assets/0176efbc-51b8-428f-bcdd-8da08ad3d1e5)

Also, by pressing 'q' we can get out form the 'less' screen
Task:

1.To calculate the flip-flop ratio:

Formula: No. of flops/no. of cells

Here, the flops are denoted by dfxtp_2

After, running synthesis, these are the statistics:
![image](https://github.com/user-attachments/assets/da6d60d7-70f6-4dc5-8727-6273bf84dd9f)

In this, dfxtp_2 = 1613 and no. of cells = 14876

Thus, the ratio is: 0.1084 and in percentage is 10.84%

