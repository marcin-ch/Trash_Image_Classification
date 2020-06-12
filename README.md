Dataset comes from:
https://github.com/garythung/trashnet/blob/master/data/dataset-resized.zip

Changes:
1. Names of the images changed (added underscore between the core name and number), e.g.
* *cardboard1.jpg* to *cardboard_1.jpg*,
* *glass2.jpg* to *glass_2.jpg* and so on
> Used *IrfanView* (`File -> Batch Conversion/Rename`)
2. All images moved to one folder (2527 in total):
* from folder *cardboard* (403 files),
* from folder *glass* (501 files),
* from folder *metal* (410 files),
* from folder *paper* (594 files),
* from folder *plastic* (482 files),
* from folder *trash* (137 files)
3. All images splitted into two folders: *train* and *test*, 80% images goes to *train* folder and 20% goes to *test* folder (images chosen randomly, manually)

Category | Train | Test | SUM
--- | --- | --- | ---
cardboard | 323 | 80 | 403
glass | 401 | 100 | 501
metal | 330 | 80 | 410
paper | 476 | 118 | 594
plastic | 386 | 96 | 482
trash | 110 | 27 | 137
***total*** | ***2026*** | ***501*** | ***2527***

4. Zipped and upload to Github as *dataset_trash.zip*
