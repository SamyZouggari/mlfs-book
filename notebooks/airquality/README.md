## Air quality project

The project is a fork from https://github.com/featurestorebook/mlfs-book

A lot of commits have been erased because I tried to do a push --force when git was broken about an hour ago (yes I panicked).

To sum up the commits that can't be seen, here is what we did : 
- running the 4 first notebooks.
- setting up a daily workflow with github actions and a dashboard with pages.
- Tried different location because we thought that a negative r-squared was exceptionnaly bad, so we thought our sensors were broken (we no longer think that).
- changed the sensor to this one.
- adding 3 features corresponding to the lag pm25 for 3 days, then for one day.

## Beginning

The first modifications were to change the .env and to put my personal API keys, to change the csv file with a sensor located in Saint-Martin-d'Hères, France (location of my former school, ENSIMAG).

After that, I run the notebooks as they were and logged the performance of the model.

MSE: 213.83423
R squared: -0.06340524613581633

I think the model is bad, but it is comprehensible since we have a few features, and that air quality could not be explained by only these features.

## Improving the model

We can think of improving the model by :
- Adjusting the ratio of test/training dataset.
- Doing some feature engineering.
- Fine tune the model.
- Adding auto-regression (later).

### Increasing the ratio train/test set
