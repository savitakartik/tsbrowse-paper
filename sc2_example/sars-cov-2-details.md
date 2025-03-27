# Details of the analysis on the SARS-CoV-2 ARG


```
$ time python3 -m tsbrowse preprocess v1-beta1_2023-02-21.pp.md.il.ts.tsz
Processing sites: 100%|█████████████████████████████████████████| 7/7 [02:15<00:00, 19.33s/it]
Writing: 100%|███████████████████████████████████████████████| 19/19 [00:00<00:00, 155.42it/s]

Preprocessing completed. You can now view with `python -m tsbrowse serve v1-beta1_2023-02-21.pp.md.il.ts.tsbrowse`

real    2m19.028s
user    15m15.049s
sys     0m8.159s
```

Sizes:

```
$ ls -lh v1-beta1_2023-02-21.pp.md.il.ts.ts*
-rw-rw-r-- 1 jk jk 130M Mar 27 15:08 v1-beta1_2023-02-21.pp.md.il.ts.tsbrowse
-rw-r--r-- 1 jk jk 113M Mar 27 15:04 v1-beta1_2023-02-21.pp.md.il.ts.tsz
```


Summary:
```
Trees   348
Sequence Length 29904.0
Time Units  days
Sample Nodes    2482157
Total Size  1.5 GiB

Table   Rows    Size    Has Metadata
Edges   2689982 82.1 MiB
Individuals 0   24 Bytes
Migrations  0   8 Bytes
Mutations   1923169 202.7 MiB
Nodes   2689054 1.1 GiB
Populations 0   8 Bytes
Provenances 1131    1.7 MiB
Sites   29803   3.1 MiB
```

Serve command:
```
$ python3 -m tsbrowse serve v1-beta1_2023-02-21.pp.md.il.ts.tsbrowse --annotations-file sc2-annotation.csv
```

