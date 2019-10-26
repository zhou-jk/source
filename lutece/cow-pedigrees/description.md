
# Content

Farmer John is considering purchasing a new herd of cows. In this new herd, each mother cow gives birth to two children. The relationships among the cows can easily be represented by one or more binary trees with a total of $N$ ($3\leq N < 200$) nodes. The trees have these properties:

* The degree of each node is $0$ or $2$. The degree is the count of the node's immediate children.
* The height of the tree is equal to $K$ ($1 < K <100$). The height is the number of nodes on the longest path from the root to any leaf; a leaf is a node with no children.

How many different possible pedigree structures are there? A pedigree is different if its tree structure differs from that of another pedigree. Output the remainder when the total number of different possible pedigrees is divided by $9901$.

# Standard Input

Line $1$: Two space-separated integers, $N$ and $K$.

# Standard Output

Line $1$: One single integer number representing the number of possible pedigrees **MODULO $9901$**.

# Samples

<style>
        table,table tr th, table tr td { border:1px solid #0094ff; }
        table { width: 200px; min-height: 25px; line-height: 25px; text-align: center; border-collapse: collapse;}   
    </style>
<table>
	<tr>
		<td>Input</td>
		<td>Output</td>
	</tr>
<tr><td>5 3</td><td>2</td></tr></table>


# Constraints



# Note

Two possible pedigrees have $5$ nodes and height equal to $3$:

```
         R                                  R
        / \                                / \
       @   @            and               @   @
      / \                                    / \
     @   @                                  @   @
```

# Source

