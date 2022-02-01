# xPEPE_Token_Viewer
 A VB.NET written interface for viewing all the MySQL data pertaining to the Tokens Offerbooks/Wallet/Balances

- Written in VB.Net by Robert Daugherty - Aka xArtist Dameinx
- Uses MySQL Data to populate datagrid's for combining data into one source for filtering and viewing
- Can be used for certain analytics as well as verifying AD's
- Join us in our Discord [HERE](https://discord.gg/HAG5Qe79wK)

Disclaimer: Please note all data is pulled via the XRP Ledger and we take no responsibility for incorrect data or issues you may experience.

- Uses data collected from [xPEPE_Token_Tool](https://github.com/xPEPENFT/xPEPE_Token_Tool)

GUI Examples

![image](https://user-images.githubusercontent.com/98682121/151728388-eb7bfe7a-2828-4319-a930-5c3d7a7392f8.png)


Wallet Data - View the Wallet ID and the current Balance of the Wallet
 - Allows for Filtering by Wallet ID and by Balance
 - Balance Filtering can be done via Equal To, Equal to Or Greater Than, Equal to Or Less Than

![image](https://user-images.githubusercontent.com/98682121/151728441-6e015806-e2ac-4c2b-8f2f-7dd08f972228.png)

Offer Book Examples
 - Seperate tabs for Sell and Buy

![image](https://user-images.githubusercontent.com/98682121/151728559-5027af09-876e-410a-998b-5ff7a280fec6.png)


Step 1 is optional (disabled by default)
 - Setting up a Users table in MySQL to force people to Login before viewing data.


Step 1: Create Users table in MySQL

```
CREATE TABLE `Users` (
  `ID` int(11) NOT NULL,
  `Username` varchar(255) NOT NULL,
  `Password` varchar(255) NOT NULL,
  `Email` varchar(255) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```

And then insert your Username/Password/Email into the table as you see fit.

Step 2: Modify the Form1.VB source code (ONLY if you have changed any of the table names/column names)
 - Will not comment further on this as if you did modify, you should know what you're doing!


Step 3: Run the program and setup your Server Settings

![image](https://user-images.githubusercontent.com/98682121/151733296-ce91c092-9d00-4108-afce-421af58245ef.png)

This is a one time input so make sure you have everything put in correctly! You will need to delete and redownload the program to clear these settings!

Step 4: Enjoy!

Examples #1 - Wallet Data
- Here you can view all the wallets that hold your Token as well as their Balance.

![image](https://user-images.githubusercontent.com/98682121/151733387-fdd4f954-913a-40fc-b622-05e8c33e5a84.png)


Examples #2 - Filtering Wallet Data
- In the options menu at the top left you'll see filtering options.
- You can filter the data by a Wallet ID or a Balance, with varying options.
- This example shows filtering by Balance of anything Equal To Or Greather Than 20 Tokens

![image](https://user-images.githubusercontent.com/98682121/151733450-66265b92-60d4-4d77-bccf-4d8cb5472bec.png)

Examples #3 - Offer Book
- You have the Sell and Buy Offer Book listed for your Token as well.
- You can filter this by wallet ID to see who is selling and who is buying your Token!

![image](https://user-images.githubusercontent.com/98682121/151733506-7c0c9075-fe81-4391-bd2e-f06ae62a329f.png)




