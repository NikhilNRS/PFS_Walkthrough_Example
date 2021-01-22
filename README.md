# Instructions for reading Walkthrough Example


This Walkthrough is intended for showing the user side of things. It mainly uses the Probabilistic Fuzzy System which can be found at: https://github.com/Nikhilrs1993/simpful and the evolution modules which is listed in the folder `modules`. 

The quickest way to get the code runnning is probably to set up a virtual env using the simpfulediting.yml file.
Alternatively, one can pip install the master branch of https://github.com/Nikhilrs1993/simpful.

**To quickly see what's possible go through the notebooks following the given order**

1. The first one uses automatic modelling for constructing the Probabilistic Fuzzy Model (PFS, using Genetic Programming).
2. The second one takes a look at the results.
3. The third one is how you would `manually` make a PFS model.


Directories/ Outline:

Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----        1/22/2021   3:52 PM                .ipynb_checkpoints
d-----        1/22/2021   9:12 AM                .vscode
d-----        1/22/2021   9:11 AM                inputs_processed_
d-----        1/22/2021   9:50 AM                modules
d-----        1/22/2021  11:07 AM                saved_models
d-----        1/22/2021   3:51 PM                saved_pickles
d-----        1/22/2021   4:00 PM                Titanic_survival_dataset(Contains preprocess steps)
-a----        1/22/2021   3:46 PM          23207 1) Titanic Model - Automatic modeling using Genetic Programming.ipynb
-a----        1/22/2021   3:53 PM         187221 2) Titanic Model Inspection.ipynb
-a----        1/22/2021   3:35 PM          11187 3) Expert defined rules.ipynb
-a----        1/22/2021   4:01 PM              0 README.md
-a----        1/22/2021  10:23 AM         101597 sample_log.log
-a----        1/22/2021   3:57 PM          10178 simpfulediting.yml


inputs_processed_ --- contains titanic sets in a processed way (X-train, X-test etc..)
modules --- contains the code for evolutions. Has some comments but needs more.
saved_models --- contains 2 already found models
saved_pickles --- Helper folder for saving intermediate results.
Titanic_survival_dataset(Contains preprocess steps) --- contains exact preprocessing steps. Consult if you're interested.

**The best way to read the notebooks is probably in the order given.**

sample_log.log --- contains (some) information about the evoltion process.

simpfulediting.yml --- **Probably quickest way to run the code**. However, the only (main) new dependency is sklearn. Specifically the confusion matrix because of the computation speed. An alternative to remove the dependency is commented out in Simpful. However it comes at the price of reduced efficiency.