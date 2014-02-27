# Sell Mastercoins for Bitcoins (currency trade offer)

Transaction Type 20: [Sell Mastercoins for Bitcoins (currency trade offer)](https://github.com/mastercoin-MSC/spec#sell-mastercoins-for-bitcoins)

Each application under test (AUT) must adhere to [The Master Protocol / Mastercoin Complete Specification](https://github.com/mastercoin-MSC/spec/blob/master/README.md) and pass the applicable tests listed in [Major Items & Scenarios To Be Tested](https://github.com/marv-engine/QA/blob/master/MastercoinDistributedExchangeTestPlan.md#major-items--scenarios-to-be-tested).

The tests for Sell Mastercoins for Bitcoins include:

1. user is able to enter valid values for all appropriate fields:
    * Currency identifier (1 for MSC, 2 for Test MSC)
    * Amount for sale
    * Amount of bitcoins desired
    * Time limit in blocks
    * Minimum bitcoin transaction fee
    * Action (1 for New, 2 for Update, 3 for Cancel)
1. valid input data is parsed and interpreted correctly, including all valid MSC Protocol transaction types in the blockchain that are supported by the AUT
1. erroneous input data, including a corrupted blockchain, is detected as not valid and handled correctly
1. correct Sell Mastercoins for Bitcoins transactions are generated from valid test input data
1. runtime error conditions are detected and handled correctly (e.g. insufficient funds, application/network/OS failure)
1. all edge cases are handled correctly
1. correct, meaningful messages reflecting transaction success/status or failure are presented to the user

For each test sequence, start in a known state and return to a known state after the test is complete. Run the tests separately and also simultaneously. The simultaneous tests should be run by the same users/addresses in the same roles where possible, and also by different users/addresses.

Where appropriate, tests should be run using the end-user UI and using the API directly.

## Positive Tests - Valid
For the positive tests, each step must succeed with correct results. 
### Basic Sell Offer manipulation
1. Create sell offer
1. Update sell offer
1. Cancel sell offer
1. Create sell offer


The tester and developer should work together to write and run procedures that thoroughly test this functionality in the AUT.

