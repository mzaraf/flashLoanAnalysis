# Aave FlashLoan Function Analysis

## Introduction

### Protocol Name: Aave
### Category: DeFi
### Smart Contract: LendingPool

## Function Analysis

### Function Name: flashLoan
### Block Explorer Link:  [Aave LendingPool Contract on Etherscan](https://etherscan.io/address/0x398ec7346dcD622eDc5ae82352F02bE94C62d119#code)

###Function Code:

function flashLoan(
    address receiverAddress,
    address[] calldata assets,
    uint256[] calldata amounts,
    uint256[] calldata modes,
    address onBehalfOf,
    bytes calldata params,
    uint16 referralCode
) external override nonReentrant {
    // Code omitted for brevity...
    address receiver = receiverAddress;
    bytes memory params = abi.encode(assets, amounts, modes, onBehalfOf, params, referralCode);
    // Code omitted for brevity...
}

