# Smart_Will
Smart_will is a Dapp that allows a person(owner) to write a will that recieves ethers and and disperse them to his/her beneficiary upon death or upon a year of inactivity or at will
the smart contract can also be used as a payment system, where addresses of workers can be added as beneficiaries
the Snart_will has two interfaces, the owner and beneficiary
the owner interface has full access to the will that allows the user to check account balance,add beneficiary, remove beneficiary, automatic distrubution of funds and the alive function
the alive function updates the timestamp of the contract, if the alive stamp has not been update for a full year, the contract interpretes as the owner is dead, and would automatically disburse the funds in the contract to all beneficiaries when any of them clicks the get lastalive function on the beneficiary interface

the beneficiary interface has only limited access, which includes the get last alive function which allows the beneficiary to know if the owner is still and automatically transfers funds to all beneficiary if owner has not been active for a full year
