# Joint Savings Account Automation

## Objective
To build a smart contract to automate the creation of and transactions related to joint savings accounts using the `solidity` language.

## Approach
Using `solidy` and the `Ethereum` network, this application will create a smart contract object containg the following properties:
* A payable address for account `one`
* Apayable address for account `two`
* The address which the last withdrawal was made to
* The last withdrawal amount and
* The current contract balance

The contract object also includes the following methods:
* `withdraw` amount to a recipient (accounts `one` or `two`)
* `deposit` which updates the balance of `this` contract
* `setAccounts` which accepts two addresses which are assigned to accounts `one` and `two`
* `anonymous` fallback function to accept payments sent outside the `deposit` method

## Testing
### Environment
The testing was carried in the `Javascript VM` provided by `Remix`.

### Results
#### Before test cases:
![State before testcases](./execution_results/01_state_before_testcases.png)

#### Test case 1: Setting up accounts `one` and `two` before:
![Setting up accounts one and two before](./execution_results/02_set_accounts_before.png)

#### Test case 1: Setting up accounts `one` and `two` after:
![Setting up accounts one and two after](./execution_results/02_set_accounts_after.png)

#### Test case 2: Depositing 1 `ether` in `wei` before:
![Depositing 1 ether in wei](./execution_results/03_send_1_ether_as_wei_before.png)

#### Test case 2: Depositing 1 `ether` in `wei` after:
![Depositing 1 ether in wei after](./execution_results/03_send_1_ether_as_wei_after.png)

#### Test case 3: Depositing 10 `ether` in `wei` before:
![Depositing 10 ether in wei before](./execution_results/04_send_10_ether_as_wei_before.png)

#### Test case 3: Depositing 10 `ether` in `wei` after:
![Depositing 10 ether in wei after](./execution_results/04_send_10_ether_as_wei_after.png)

#### Test case 4: Depositing 5 `ether` before:
![Depositing 5 ether before](./execution_results/05_send_5_ether_before.png)

#### Test case 4: Depositing 5 `ether` after:
![Depositing 5 ether after](./execution_results/05_send_5_ether_after.png)

#### Test case 5: Withdrawing 5 `ether` from account `one` before:
![Withdrawing 5 ether from account 1 before](./execution_results/06_withdraw_5_accountOne_before.png)

#### Test case 5: Withdrawing 5 `ether` from account `one` after:
![Withdrawing 5 ether from account 1 after](./execution_results/06_withdraw_5_accountOne_after.png)

#### Test case 6: Withdrawing 10 `ether` from account `two` before:
![Withdrawing 10 ether from account 2 before](./execution_results/07_withdraw_10_accountTwo_before.png)

#### Test case 6: Withdrawing 10 `ether` from account `two` after:
![Withdrawing 10 ether from account 2 after](./execution_results/07_withdraw_10_accountTwo_after.png)
