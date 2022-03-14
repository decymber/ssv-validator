   ```text                                                               
                  #####     #####                                 
                ##     #####     ##                               
    ###         ##   #######     #########################        
    ##  ##      #####               ##                   ##       
    ##     #####                 ##                       ##      
    ##     ##                     ##                      ###     
   ########                        ##                     ####    
   ##        ##   ###         #####                       #####   
   #                          ##                         # #####  
   #                            #                        #  ##### 
   ##                             ##                    ##        
   ##                              ##                   ##        
   ##             ###              ##                   ##        
   ###############                 ##                   ##        
   ###               ##                                 ##        
      #############################                    ##         
                     ##                             ###           
                     #######     #################     ###        
                     ##   ## ##        ##   ##    ###             
                     ##############          #############        
```                         
                         
# ssv-deposit-cli

## Build the docker image
`docker build -t ssv-deposit-cli .`

## Create keys and deposit_data-*.json
Create a directory to hold the created keys
`mkdir -p $HOME/.ssv`

Run the following command to enter the interactive CLI:
`docker run -it --rm -v ~/.ssv/validator_keys:/app/validator_keys ssv-deposit-cli new-mnemonic --num_validators=1 --mnemonic_language=english --chain=prater`

See results:
```text
Creating your keys.
Creating your keystores:	  [####################################]  1/1
Verifying your keystores:	  [####################################]  1/1
Verifying your deposits:	  [####################################]  1/1

Success!
Your keys can be found at: /app/validator_keys


Press any key.
The generated files have been copied to ./.ssv/validator_keys/
```

