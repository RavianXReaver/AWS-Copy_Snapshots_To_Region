## Usage

```shell
OPTIONS:
Required:
-s      string  Source Region of the Snapshot
-d      string  Destination Region of the Snapshot
-m      string  Description of the Snapshot
 
Either: Select only one parameter
-i      string  ID of the Snapshot
-e      string  Path to the CSV which contains list of snapshot IDs"
```
## Example

### Single Snapshot
```shell
./CopySnapshot -s ap-southeast-1 -d ap-south-1 -m "Ansible Server - dev" -i snap-123a34359f8a8e8u2
```

### Multiple Snapshots from CSV
```shell
./CopySnapshot -s ap-southeast-1 -d ap-south-1 -m "Ansible Server - dev" -e /your/path/to.csv
```
