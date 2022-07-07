# make_nexus_for_iqtree

Make nexus file from multiple fasta files generated by tools such as Orthofinder.

## Usage

```
python make_nexus_for_iqtree.py -s [suffix name] -i [path to directory]
```

`partition.nexus` will be generated.

After this, execute iq-tree, for example.

```
iqtree -sp partition.nexus -nt AUTO -bb 1000 -m MFP -alrt 1000
```

## Example

```
python make_nexus_for_iqtree.py -s fa.trimal.aln.renamed.fa -i /path/to/directory/of/fasta/files
```
