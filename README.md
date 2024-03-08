**InnovativeClub Smart contract**

**Overview:**
The InnovativeClub smart contract is designed to manage membership registrations and selections for an exclusive club. It operates on the Ethereum blockchain platform, utilizing Solidity programming language.

**Features:**

1. **Joining Fee:** 
   - The contract allows setting a joining fee, which members must pay to join the club. 
   - The joining fee can be any amount up to 1000 units (not specified).
   - Premium membership is offered for joining fees exceeding 500 units.

2. **Registration:**
   - The `registration` function enables individuals to register as members by paying the joining fee.
   - It checks that the joining fee is within acceptable limits (<= 1000 units).
   - If the joining fee exceeds 500 units, it grants premium membership and restricts further registration.

3. **Selection Process:**
   - The `selectPerson` function is used to select individuals who have successfully cracked an interview or met specific criteria.
   - Eligible individuals are identified by setting the `_crackedInterview` parameter to true.
   - Only those who have successfully passed the interview process can join the club.

4. **Membership Tracking:**
   - The contract maintains a mapping of members, tracking whether they have cracked the interview or not.
   - The `members` mapping stores this information using the Ethereum addresses of the members as keys.

**Usage:**

1. **Registration:**
   - To register, call the `registration` function with the desired joining fee as a parameter.
   - Ensure that the joining fee is within the allowed limit.
   - If opting for premium membership, pay a fee greater than 500 units.

2. **Selection:**
   - The club administrators can use the `selectPerson` function to admit individuals who have successfully cracked the interview.
   - Pass the address of the individual and set `_crackedInterview` to true to allow membership.

**License:**
This smart contract is provided under an **UNLICENSED** SPDX-License-Identifier. 

**Author**

Darshan

dharshan98760@gmail.com
