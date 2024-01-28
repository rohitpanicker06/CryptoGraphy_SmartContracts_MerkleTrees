To Code base contains a merkle proof generator and a verifier generator.

1. To run the prove phase run the following command
run --package Cryptography_Assignment_2_MerkleTrees --bin Cryptography_Assignment_2_MerkleTrees prove 100 95

here 100 denotes the number of leaf nodes and 95 denotes the leaf node position
Running the prove phase will create a merkle proof which is flushed into a yaml file named proof_gen_{num_of_leaves}_{leaf_pos}.yaml
It will also generate and print the merkle root hash to the console


2. To run the verifier phase, run the following command
run --package Cryptography_Assignment_2_MerkleTrees --bin Cryptography_Assignment_2_MerkleTrees verify proof_gen_{num_of_leaves}_{leaf_pos}.yaml {merkle_root_hash}
