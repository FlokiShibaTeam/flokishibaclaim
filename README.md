
# Infomation and rule

1. Folder name tokenList.json is a list campaign.
    
    `How to add an token.`
    ```
    - Create a file name tokenList.json and write data.
    - name, symbol, address, decimals, chainId, logoURI is info of token.
    - position is location of token to display.
    - Example: 
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
    
    * Attention: chainId is 56
    ```

2. /root folder is storage place address list.

      `Structure`
      ```
      root/<tokenAddress>/<tokenId>.json
      ```
      Replace <tokenAddress> by token address.
      
      Replace <tokenId> by token id.
  
2. Example: 
      
      Token address: 0x0C3898ABdBE317C10a07fe4913836de3851CbaFC
      
      Token Id: 180987475

      `path file:`
      ```
      root/0x0C3898ABdBE317C10a07fe4913836de3851CbaFC/180987475.json
      ```

## Rule

      1. Required json file.
      
      2. Folder name and token name is not discus uppercase and lowercase.
