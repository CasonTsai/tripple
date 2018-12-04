## Face Project
### Train
```python
python train.py -net mobilefacenet
```
data available in 238
***
### Test
extract gallery features save in .pkl 
```python
python eval_data.py --net mobileface --imgdir path --phase extra
```
calculate the similarity between test image and gallerys, and classification
```python
python eval_data.py --net mobileface --imgdir test-path --phase eval
```
two model available right now:

./work_space/model
***
## Face Verification results

model | capacity | agedb_30 | cfp_fp | lfw
---|---|--- |--- |---|
sphereface | 107M | 93.56 | 95.04 | 99.42
mobileface | 4.6M | 90.63 | 93.05 | 99.24


***
modify by [InsightFace](https://github.com/TreB1eN/InsightFace_Pytorch)