## Chains

Chains are composed of a [root](#root), a [tip](#tip) and all blocks in
along the path from the tip block to root block.

### Main chain

Chain whose [tip](#tip) has the largest [chain work](#chain-work) and
whose [root](#root) is the [genesis block](#genesis-block). 

Also referred to as the Blockchain.

### Side chains

Chains whose [chain work](#chain-work) is lower that of the [main chain][#main-chain].

### Orphan chains

Chains whose root is an [orphan block](#orphan-block).

### Chain work

The combined work that went into a block and all its preceding blocks.

It is recursively defined as: 

chain work = previous block's chain work + block's [work](#work)

### Height

The height of a block within a chain is measured as the number of blocks that precede
it.

The height of a chain is the height of its tip.

### Tip

A tip is informally known as the last block of a chain. It is defined
as a block who is not the previous block of any other block.

### Root

A root is informally known as the last first block of a chain. It is defined
as a block who has no previous block.

### Orphan block

A block who's previous block is not known. The [genesis block](#genesis-block) 
is an exception and is not considered an orphan block.

### Genesis block

Block that is hard coded as the first valid block in Bitcoin's original client.
Bitcoin's genesis block hash is
`000000000019d6689c085ae165831e934ff763ae46a2a6c172b3f1b60a8ce26f`.

## Blocks


### Work

Informally, it represents how much computational power has gone into
creating the block. Defined as:

(# of possible hashes) / (target + 1)

### Target

TODO.......
