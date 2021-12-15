# Miscellaneous Quirks

## Downloading apps from Underground

By default, Underground uses a BitTorrent-like approach to downloading files. First, Underground SHA-1 hashes the file being downloaded. Then, this *hash* is checked against a database of apps and hashes, by default one by us. Next, the network is scanned for files with matching hashes as reported by the database. If Underground finds a match on a server closer to the user, it downloads it from there instead. For added security, the final file is also hashed and verified by Underground before downloading it. (The original file's `Torchfile` settings are parsed and used to make the eperience more seamless.)
