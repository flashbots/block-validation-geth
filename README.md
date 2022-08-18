[original readme](README.original.md)

# Block validation API

Geth with additional RPC method `flashbots_validateBuilderSubmissionV1`.  
The new method accepts `github.com/flashbots/go-boost-utils/types.BuilderSubmitBlockRequest` - boost relay builders' block submission.  
It will ensure that the block is valid and that it transfers the expected funds to the fee recipient.  

This code is *not* production ready. Do not use in production environments.  

