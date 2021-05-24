# First Order Motion Model for Image Animation


### Installation

We support ```python3```. To install the dependencies run:
```
pip install -r requirements.txt
```

### Pre-trained checkpoint
Checkpoints can be found under following link: [google-drive](https://drive.google.com/open?id=1PyQJmkdCsAkOYwUyaj_l-l0as-iLDgeH) or [yandex-disk](https://yadi.sk/d/lEw8uRm140L_eQ).
You can download vox-adv-cpk.pth.Place it in checkpoint directory.

### Animation Demo
To run a demo, download checkpoint and run the following command:
```
python demo.py  --config config/dataset_name.yaml --driving_video path/to/driving --source_image path/to/source --checkpoint path/to/checkpoint --relative --adapt_scale
```
The result will be stored in ```result.mp4```.
If you want to define any form of expression, you can run the following command:
```
python camera_demo.py --config config/vox-adv-256.yaml --source_image demo/lp.png --checkpoint checkpoint/vox-adv-cpk.pth.tar --relative --adapt_scale --cpu
```
The result will be stored in ```result1.mp4```.


#### Additional notes

Citation:

```
@InProceedings{Siarohin_2019_NeurIPS,
  author={Siarohin, Aliaksandr and Lathuilière, Stéphane and Tulyakov, Sergey and Ricci, Elisa and Sebe, Nicu},
  title={First Order Motion Model for Image Animation},
  booktitle = {Conference on Neural Information Processing Systems (NeurIPS)},
  month = {December},
  year = {2019}
}
```
