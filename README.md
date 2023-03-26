# Smart_Will
Smart_will is a Dapp that allows a person(owner) to write a will that recieves ethers and and disperse them to his/her beneficiary upon death or upon a year of inactivity or at will.
the smart contract can also be used as a payment system, where addresses of workers can be added as beneficiaries
the Smart_will has two interfaces, the owner and beneficiary
the owner interface has full access to the will that allows the user to check account balance,add beneficiary, remove beneficiary, automatic distrubution of funds and the alive function
the alive function updates the timestamp of the contract, if the alive stamp has not been update for a full year, the contract interpretes as the owner is dead, and would automatically disburse the funds in the contract to all beneficiaries when any of them clicks the get lastalive function on the beneficiary interface

the beneficiary interface has only limited access, which includes the get last alive function which allows the beneficiary to know if the owner is still alive and automatically transfers funds to all beneficiary if owner has not been active for a full year.

#Note
the html code for the beneficiary page can be found on; https://github.com/code-xiake/smart_will2 i decided to split it, because i was having trouble uploading the full repo on vercel.
there are also two seperate front ends, because i didnt want the benefiaciary to get access to the owner functions, even though all transactions will revert if mgs.sender is not owner
in the original deployed contract there is a self destruct function but after deploy the contract i decided not to include that function on the frnt end, because i didnt want it to be mistakenly clicked.thanks


deployment details;
contract address;0xCA24c7a01095A698Ae3679F5c78e9e656F18f170 
live site for owner;https://smart-will-code-xiake.vercel.app/
live site for beneficiary; https://smart-will2.vercel.app/

note to grader; the contract was deployed with the graders test address on goerli as the owner, if said address is wrong, kindly reach out before grading.
graders address; 0xa1B94ef0f24d7F4fd02285EFcb9202E6C6EC655B
