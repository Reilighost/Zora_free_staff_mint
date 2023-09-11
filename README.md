
# Zora-free-mint script created by [BBC™](https://t.me/CryptoBub_ble) 

## Overview

This script is designed to automate the minting of NFTs on the Zora Network. It utilizes different accounts, each with its own time delay between transactions and a target transaction count. Each account will mint tokens until it reaches its target count, adhering to the specified delay between transactions.

Use this collection as a mint-poll:

[A Great Day](https://mint.fun/zora/0x4de73D198598C3B4942E95657a12cBc399E4aDB5) - [Allure](https://mint.fun/zora/0x53cb0B849491590CaB2cc44AF8c20e68e21fc36D) - [Cosmic Girl](https://mint.fun/zora/0xca5F4088c11B51c5D2B9FE5e5Bc11F1aff2C4dA7) -
[Fla](https://mint.fun/zora/0x9eAE90902a68584E93a83D7638D3a95ac67FC446) - [GoldenFla](https://mint.fun/zora/0x4073a52A3fc328D489534Ab908347eC1FcB18f7f) - [Whimsical Euphoria: A White Inflatable Sheep](https://mint.fun/zora/0x12B93dA6865B035AE7151067C8d264Af2ae4be8E) -
[Zora Mafia](https://mint.fun/zora/0xC47ADb3e5dC59FC3B41d92205ABa356830b44a93) - [ZoraEye NFT](https://mint.fun/zora/0x8A43793D26b5DBd5133b78A85b0DEF8fB8Fce9B3) - [Zora OG Pass](https://mint.fun/zora/0x266b7E8Df0368Dd4006bE5469DD4EE13EA53d3a4) -
[Zora Cola Classic](https://mint.fun/zora/0xFa177a7eDC2518E70F8f8Ee159fA355D6b727257) - [Dithered Zorb](https://mint.fun/zora/0x48D913ee06B66599789F056A0e48Bb45Caf3b4e9) - [AUDREY ZORA](https://mint.fun/zora/0x29519d48612E11D9cEFB006D82A35a8481e1ABdB) -
[Zoggles](https://mint.fun/zora/0x8974B96dA5886Ed636962F66a6456DC39118A140) - [sqr(16)](https://mint.fun/zora/0xbC2cA61440fAF65a9868295Efa5d5D87c55B9529) - [ZORA NFT CRYSTAL](https://mint.fun/zora/0xb096832A6ccD9053fe7a0EF075191Fe342D1AB75) -
[Zorbee](https://mint.fun/zora/0x8f1B6776963bFcaa26f4e2a41289cFc3F50eD554) - [DriftBottleSeeds](https://mint.fun/zora/0xd46760C832960eEBd81391aC5DC8502A778B24Ec) - [TEXT](https://mint.fun/zora/0xA46aE6ffa6D987eeAF704E8ff6268Fc8D8166e1c) -
[Dragon Zorb](https://mint.fun/zora/0x93BCe2fF7CF7cFc722F70F8a5A93C2849C5eDEEF) - [Opepen Rug Edition](https://mint.fun/zora/0x6BF820b6EF66B9946d078679a50DcDF2BF2e033c) - [Web3 Flower](https://mint.fun/zora/0x438F8f41801d470d0b7551F4d01853e7ca1fd0D8) -
[Witchcraft](https://mint.fun/zora/0x300Ee523E8b95B3B4DB763089505F525a2d61721) - [Sonic Zorb](https://mint.fun/zora/0xb3d0bA3c295FdB0918Fe4BcDE04f62f36E60F50c) - [Web3 PunkGirl](https://mint.fun/zora/0xdB123EeDcFE960a03310D3A26f4A28D26627dcfe)


## Features

- **Automated Minting**: Continuously mints tokens using the provided private keys.
- **Account-specific Configurations**: Each account has its own time delay and target transaction count.
- **Proxy Support**: Utilizes proxies to bypass geographical RPC restrictions, especially relevant for users in countries like Russia)
- **Gas Optimization**: Use a special trick to decrease gas price by 30 times, down to `0.01-0.03$` per mint, make each gas setting unique to avoid detection.

## Configuration

### `config.json`

This file provides the main configurations:

- **Contract**: The Zora Network contract address and quantity to mint.
- **Account Delay**: The delay (in hours) between transactions for each account.
- **Target Transactions**: The target number of transactions (minting operations) for each account.

### External Files

- `pkey.txt`: Contains a list of private keys. Used to populate the initial Excel sheet.
- `proxies.txt`: Contains proxy details, which are used to bypass RPC restrictions. If the number of proxies is not enough for the wallets, the list will extend to ensure coverage.

**Note**: Once the Excel file is created, `pkey.txt` and `proxies.txt` can be deleted for security reasons.

## Installation

To run the script, ensure you have the necessary Python libraries installed:

```
git clone https://github.com/Reilighost/Zora_freemint.git

pip install pandas requests web3 colorlog logging colorama openpyxl

cd Zora_freemint

python main.py

```

## Usage

1. Populate the `pkey.txt` and `proxies.txt` files.
2. Adjust the configurations in `config.json` as needed.
3. Run the script. It will automatically mint tokens using the provided accounts, adhering to each account's delay and target transaction count.
4. You need to be subscribe for 
## Security Considerations

It's crucial to handle private keys with care. Once the Excel file with account details has been generated, it's recommended to delete the `pkey.txt` file to safeguard the private keys.


