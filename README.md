1. Load dicom files into volume [series]
2. Simple alg function [application] - MIP from volume
3. Create worker that embeds alg function
4. Run worker on k8s - use k8s rust api to create deployment
5. Worker should iterate over s3fs files and run algo, save results in s3fs bucket
6. Worker should connect redis and process a list of series
7 Process - create a list of dicom seris by iterating s3fs and upload the list to redis.
