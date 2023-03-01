# Full-Stack-Web3--CrowdFunding-DApp

This is a Solidity smart contract for a crowdfunding platform.

The contract defines a struct Campaign, which stores information about each crowdfunding campaign, such as the owner's address, the title and description of the campaign, the target amount of funds to raise, the deadline for the campaign, the amount of funds collected so far, an image for the campaign, and arrays of addresses and donation amounts for each donor.

The contract also defines a mapping campaigns that maps campaign IDs to Campaign structs. The contract keeps track of the number of campaigns with the numberOfCampaigns variable.

The createCampaign function creates a new crowdfunding campaign by initializing a new Campaign struct and adding it to the campaigns mapping.

The donateToCampaign function allows donors to contribute funds to a campaign by sending ether with the function call. The function adds the donor's address and the amount donated to the appropriate arrays in the Campaign struct and updates the amountCollected field.

The getDonators function returns the arrays of donor addresses and donation amounts for a given campaign ID.

The getCampaigns function returns an array of all the Campaign structs stored in the contract.




