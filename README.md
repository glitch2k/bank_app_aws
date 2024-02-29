# objective
## initial deployment of a bank account api
        perform bank teller operations
            create a new member account
                input
                    member's fill name
                    member's phone number
                    member's initial deposit
                        must be greater than $50

                process
                    validate the input date
                    generate a account number that is not already used
                    create a record for the account with the following fields
                        acct_num
                        f_name
                        l_name
                        tel_num
                        balance

                output
                    standard http response message
                        status (required)
                        body (required)
                            object that represents the member's account
                        status_text (required)
                        headers
                
            deposit money into a member's account
                input
                    member account number
                    amount to be deposit

                process
                    validate the input date
                    validate that the member's account exist
                    get the current balance of the member's account
                    calculate the new balance
                    update the member's account with the new balance

                output
                    standard http response message
                        status (required)
                        body (required)
                            object that represents the member's account
                        status_text (required)
                        headers

            withdraw money from a member's account
                input
                    member account number
                    amount to withdraw

                process
                    validate the input date
                    validate that the member's account exist
                    get the current balance of the member's account
                    validate the member has enough money to withdraw
                    calculate the new balance
                    update the member's account with the new balance

                output
                    standard http response message
                        status (required)
                        body (required)
                            object that represents the member's account
                        status_text (required)
                        headers
                        
            display the status of a member's account
                input
                    member account number

                process
                    validate the input date
                    validate that the member's account exist
                    get the record for the member's account

                output
                    standard http response message
                        status (required)
                        body (required)
                            object that represents the member's account
                        status_text (required)
                        headers

## feature adds
      perform bank manager operations
            report on bank accounts
                input
                    member account number

                process
                    validate the input date
                    validate that the member's account exist
                    get the record for the member's account

                output
                    standard http response message
                        status (required)
                        body (required)
                            object that represents the member's account
                        status_text (required)
                        headers
