Honeybees are the world's most important pollinator of food crops. There are fears that this important species is being threatened by climate change. This project uses pregenerated datasets from the iNaturalist citizen science project to monitor the number of observations of honeybees in the state of Maryland since the inception of the project to the latest observation. The resulting graphs are shown by season and year and are adjusted by number of contributors, as the number of users of iNaturalist increases as its popularity increases.

This python code can be reused to monitor the observation of any other species using data from iNaturalist, and the location can also be changed, broadened, or made more localized. In our examples, we test the reusability with butterflies, another important pollinator. 



## Step 1: download pregenerated dataset for honeybees in the state of Maryland from iNaturalist as follows:
1. Go to iNaturalist.org and sign into your account.
2. Go to observations > export and create a Query with the following criteria in the following fields:

    Filter: quality grade Research
    
    Place: DMV, US
    
    Taxon: Apis mellifera
    
3. Create export

## Step2: unzip, upload, and import dataset as iNat_monitor:
Upload example: iNat_monitor = pd.read_csv('observations-71449.csv', header=0, parse_dates=True, squeeze=True)

## Further steps: run python program DMV_bees.ipynb