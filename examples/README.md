# Examples

Sample configuration files of the kind described in the main [README](../README.md).
IDs and paths are illustrative placeholders rather than real values.

## `config.xml`

Maps image files on disk to the player IDs the software uses as database keys.
Each `<record>` inside `<list id="maps">` ties one ID to the path of its portrait.

The mapping only resolves if the ID in the config, the folder name, and the
database key all agree exactly — a single mistyped digit and the software falls
back to a blank portrait without reporting an error.
