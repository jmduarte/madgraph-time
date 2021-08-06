# madgraph-time

User docker container: [hfukuda/madgraph](https://hub.docker.com/r/hfukuda/madgraph).

To recreate the `ppTOgg_13TeV` directory:
```bash
/home/hep/MG5_aMC_v2_6_3_2/bin/mg5_aMC 
```

Then at the madgraph prompt, do:
```
generate p p > g g
output ppTOgg_13TeV
launch ppTOgg_13TeV
shower=Pythia8
run_card_ptbin.dat
```

Or skip that and just do
 ```bash
cd ppTOgg_13TeV
time ./bin/generate_events  -f
 ```
