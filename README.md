# Infomation and rule

1. Folder name tokenList.json is a campaign list.
    
    `How to add an token.`
    
    ```
    # Step 1: Add token to tokenList.json.
    
        $ (name, symbol, address, decimals, chainId, logoURI) is info of token.
        $ (position) is location of token to display.
        
      Example: tokenList.json.
    
        {
          "tokens": [
            {
              "name": "HORA Os",
              "symbol": "HORA",
              "address": "0xa6fd7b5c9eee30309b00b65436a284e2053251e5",
              "chainId": 56,
              "decimals": 18,
              "position": 5,
              "logoURI": "https://raw.githubusercontent.com/HoraOS/media/main/LOGO%20HORA%20OS.png"
            },
            {
              "name": "Token B",
              "symbol": "Token b",
              ...
              ...
            }
          ]
        }
    
    # Step 2: Add token in https://claim.flokishiba.com/#/partner
    
    a. Click button (Add Campaign), inside: 
    
        $ Token Address is address of token. -> 0x....
        $ Total Campaign Amount is total campaignn amount for an campaign -> Number
        $ Amount Per each claimer is amount for each claim -> Number

    b. Click confirm transaction and accept on metamask.
    
    * Attention: chainId is 56
    
    ```

2. /root folder is storage place address lists is accept claim.

      `Structure`
      
      ```
      root/[tokenAddress]/[tokenId].json
      ```
      Replace [tokenAddress] by token address campaign.
      
      Replace [tokenId] by token id campaign.
  
      `Example`
      
      Token address: 0x1a26613d922cBb776887BCF91dAf45Ac44da6aeA
      
      Token Id: 180987475

      `path file:`
      
      ```
      root/0x1a26613d922cBb776887BCF91dAf45Ac44da6aeA/180987475.json
      ```

      `Data in path file:`
      
      ```
      0x1a26613d922cBb776887BCF91dAf45Ac44da6aeA is address of user. 
      
      {
        '0x1a26613d922cBb776887BCF91dAf45Ac44da6aeA': 1,
        'user 2': 1,
        'user 3': 1,
        ...
      }
      ```
      
## Rule

      1. Required json file.
      
      2. Folder name and token name is not discus uppercase and lowercase.


