If you update a json application, please unminify it for sensible diffs.

Use exactly these options:
```sh
json_pp -json_opt=canonical,indent,ascii
```

E.g.
```sh
cat your-minified-export.json | json_pp -json_opt=canonical,indent,ascii > beautiful.json
```

Option "canonical" makes hashmap key order deterministic, so entries don't move around.
Option "indent" provides the line breaks and indentations.
Option "ascii" enables proper escaping of all unicode characters (technically, without that
option, the result might not be valid JSON at all).

