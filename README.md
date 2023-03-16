# Archived: This repo is no longer used by flashbots.

This repo is deprecated in favor of the validation API in the flashbots builder.

Use https://github.com/flashbots/builder for block validation.

[original readme](README.original.md)

# Block validation API

Geth with additional RPC method `flashbots_validateBuilderSubmissionV1`.  
The new method accepts `github.com/flashbots/go-boost-utils/types.BuilderSubmitBlockRequest` - boost relay builders' block submission.  
It will ensure that the block is valid and that it transfers the expected funds to the fee recipient.  

## Blacklisting

By default the node will load blacklisted addresses from `ofac_blacklist.json` from working directory. You can specify the path to the file via `--builder.validation_blacklist`.  

The default OFAC blacklist is provided with this repository in [ofac_blacklist.json](ofac_blacklist.json).  
